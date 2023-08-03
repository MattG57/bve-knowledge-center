### Development Speed and Code Security
@MattG57

# Considerations for improving both Development Speed and Code Security

_Authors:  Matthew Gunter  
Last Edited: May 9th, 2022_



## 📏 Code Scanning Effectiveness
The effectiveness of Code Scanning can be defined in terms of **Security Risk Reduction**. 

We find evidence for such improvements with *GitHub Advanced Security* as shown by the recent Forrester TEI research<sup>1</sup>. For example, they cite the following survey results:

  <span class="indented" style="padding-left: 75px;">![security flaws](/bve-knowledge-center/assets/img/security-flaws.png){:height="600px" :width="600px" :border="2px"}</span>
  



Yet, Code Scanning, by itself, does not reduce risk. Scanning also requires developers to quickly remediate problems to efficiently and sustainably reduce the vulnerability backlog and thereby improve Software Risk.

...Wait, Why do Developers need to move quickly? ( This can seem counterintuitive if security is associated with being slow, cautious and deliberate. )

Code Scanning requires Speed of Remediation.

This becomes important for a few key reasons:

A vulnerability backlog already exists that must be reduced (that’s the Risk Reduction)
The backlog exists because new vulnerabilities have been discovered faster than they have been remediated
New vulnerabilities arise for three reasons: code changes introduce a vulnerability, new CVE’s are discovered, and when dependencies are updated. Orgs can only slow down code changes, but not the other two sources.
The rate of remediation must overtake the rate of introduction of new vulnerabilities and therefore reduce the overall size of the Vulnerability Backlog.

These two charts may help clarify what these metrics mean:

(Graphic: How the Vulnerability Picture Changes with Time)

(Graphic: How the Rate of Remediation impacts Backlog & Risk)

The graphic on the left shows how a current backlog may change between PRs. New Vulnerabilities (and new Remediations) can add to (or subtract from) the Backlog at each PR. These vulnerabilities can have various criticalities and they can arise from either local code changes or from introductions of new CVE’s or from updated Dependencies.

On the right-side it shows the count of new vulnerabilities and new remediations over time. If the rates are different, and remediation happens at a slower rate, it will cause the backlog to continue growing. This is why speed matters. Rate of Remediation often needs to increase.

<sup>1</sup> https://resources.github.com/forrester/


## 📊 Acceleration of Application Security Risk
The vulnerability backlog that many teams have inherited, often seems overwhelming. Even a one-time “bug-bash” approach may only make a dent in the backlog of vulnerabilities. This means that a sustained, and sustainable, effort is clearly needed.

Scanning, by itself - no matter how precise or comprehensive, isn’t enough.

Instead, Teams will need to deliver remediations at a faster pace to catch up.

The following industry evidence implies that the (via minimizing the vulnerability backlog)

a. CVE's are rising every year

(https://nvd.nist.gov/general/visualizations/vulnerability-visualizations/cvss-severity-distribution-over-time )

b. Sonatype's Open Source Project Quality Metric, MTTU (mean time to update), shows maven dependencies updating more frequently. Typical open source projects have increased update frequency from ~1 time per year in 2011 to ~12 times a year in 2021. (see attached SSSC-Report)

c. Faster updates correlate with fewer vulnerabilities: "As in previous studies, we see a strong correlation between better update hygiene, as measured by MTTU, and security, as measured by lower rates of “vulnerabilities” (see attached SSSC-Report)

d. Organizations are scanning applications more frequently: " A decade ago applications were scanned two or three times a year. Now, 90 percent of applications are scanned more than once a week with the majority scanned three times a week." (see attached Veracode SOSS report )

August 2022 Page 3

## 📉 Reduce Security Risk
Without adding developers, there are three primary ways that rate of remediation can be increased. :

a. Shifting a larger portion of each developer's time to remediation. (creates a controversial trade-off between security and delivery of features)

b. Reduce the amount of time per remediation. (This is the non-controversial approach and translates to other desirable improvements in the SDLC)

c Pursue both (a) and (b). ( If reducing the amount of time per remediation improves productivity, then dev speed and security are both improved.)

How can reducing the "amount of time per remediation" ( in (b) ) be accomplished?

There are several techniques and process improvements supported by GHAS that can make remediation more efficient. Several of them are listed below (along with evidence for their relevance) to consider:

d. Integrate scanning into PR process:

Shifting Left is known to reduce cost per vulnerability, which is largely the same as amount of time required for remediation.

e. Minimize False Positives ( or Noise ) reduces developer effort:

"Fewer False Positives, mean fewer workflow interruptions" (Quote from Netdata, a GitHub advanced security customer)

f. Minimize solution complexity improves coordination:

"If you run detection, analysis, and remediation outside GitHub and you find an issue, you have the added complexity of answering questions like: Who checked in the code? Who’s the owner? When was the last commit?” (Quote from Hashicorp, a GitHub advanced security customer )

g. Maximize Visibility to empower better decisions:

"It brings a level of visibility that helps everyone in the value chain do their best.” (Quote from Infosys, a GitHub advanced security customer)

h. Maximize Coverage to avoid Future Surprises:

GitHub & GHAS have the ability to protect against Code, Dependency and Secret-related vulnerability types. If dependencies are found downstream, it defeats the purpose of Shifting Left, so having broad coverage is key. CodeQL is also constantly updated with new queries to detect new vulnerabilities, some new queries are developed internally and some are contributed via the community-driven bounty program.

i. Don't allow Coverage and Developer Visibility to become trade-offs:

Instead, integrate 3rd party scanning execution and reporting into GHAS, so that developer visibility(and esp. responsibility) is maintained. ( When Secure Code Warriors surveyed Developers about why vulnerabilities may knowingly be deployed, 25% claimed that finding and fixing insecure code was the responsibility of someone else. (see attached report: The_challenges_and_opportunities_to_improve_software_security_FINAL )

(Screen shot showing 3rd party scan results displayed in GitHub)

How much will the rate of remediation be improved using the recommendations above?

j. How much time is being spent per remediation today? How effectively is that time being used?

k. Will these improvements help with the current backlog of vulnerabilities?

Shifting Left will primarily have an effect on newly created vulnerabilities that are caught at PR time. Vulnerabilities from the backlog will benefit from the process improvements, mentioned above, such as more precise scan results, less complexity, more visibility, better coverage, and extensibility.

l. What rate of remediation should be targeted?

The best answer is the rate that allows your vulnerability backlog (esp. high and critical findings) to be brought down to near zero. A blacklog level much greater than zero, or worse, a growing backlog, indicates the rate of remediation is too slow to keep up with development and CVE growth.

m. What has GitHub seen in other scenarios?

For Dependabot-enabled repos, the MTTR (mean time to remediation) drops from an industry average of 180 days down to 40 days. This means that ~4 Times as many vulnerabilities can be addressed in the same time period.

n. What have other customers seen?

Compared to previous scan tooling, GHAS eliminated 23 false positives and 3 false negatives. When this improvement is applied across the orgs 36 critical repos, the MTTR for vulnerabilities is expected to be 1/3rd the current MTTR. This translates to 3 times the number of vulnerabilities remediated in the same time period.



1. What information might this feature expose to Web sites or other parties, and for what purposes is that exposure necessary?

This feature exposes the same partitioned information available in an iframe to a top-level frame, but prevents the top-level frame with this access from using unpartitioned information.
This exposure is necessary for some login flows and other contexts where popups need access only to partitioned data.

2. Do features in your specification expose the minimum amount of information necessary to enable their intended uses?

Yes, as we prevent the top-level frame with access to partitioned data from gaining access to unpartitioned data as well.

3. How do the features in your specification deal with personal information, personally-identifiable information (PII), or information derived from them?

N/A

4. How do the features in your specification deal with sensitive information?

N/A

5. Do the features in your specification introduce new state for an origin that persists across browsing sessions?

No.

6. Do the features in your specification expose information about the underlying platform to origins?

No.

7. Does this specification allow an origin to send data to the underlying platform?

No.

8. Do features in this specification enable access to device sensors?

Yes, the same access to device sensors already possible from a top-level frame are also accessible to this top-level frame.

9. Do features in this specification enable new script execution/loading mechanisms?

No.

10. Do features in this specification allow an origin to access other devices?

No.

11. Do features in this specification allow an origin some measure of control over a user agent’s native UI?

Yes, the ‘partitioned popin’ is a new variant of popup which can interrupt a browsing session on a particular origin.

12. What temporary identifiers do the features in this specification create or expose to the web?

N/A

13. How does this specification distinguish between behavior in first-party and third-party contexts?

First-party contexts must delegate this feature to third-party contexts for them to use it.

14. How do the features in this specification work in the context of a browser’s Private Browsing or Incognito mode?

This feature works the same between different browsing modes.

15. Does this specification have both "Security Considerations" and "Privacy Considerations" sections?

The explainer has this section.

16. Do features in your specification enable origins to downgrade default security protections?

Yes, it is possible to delegate this feature to * instead of sticking to self or delegating only to specific origins.

17. How does your feature handle non-"fully active" documents?

Documents must have committed their navigation and be executing scripts to open a popin.

18. What should this questionnaire have asked?

N/A

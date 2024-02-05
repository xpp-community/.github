# XPP Community

We encourage our userbase to share ideas through repositories hosted here. By sharing data to this Github account, you agree to abide by the RWS Community Terms and Conditions outlined here:   https://www.rws.com/legal/terms-and-conditions/community-terms-conditions/

## Repository Best Practices

### Readme

Provide a Markdown README.md file at the root of the repository. This readme can either summarize the goal of the JOB, or, if appropriate, you may use the entirety of the content for the JOB/DIVs (be aware that if you have an HTML version of such content, you can use various HTML→Markdown converters available online. While not required, consider the inclusion of a DIV_readme as well, which is an XPP rendering of the same content.

Suggested Readme content:

- explain the functionality the JOB sample is demonstrating
- explain what each of its member DIVs are demonstrating
- explain any steps needed to view/output sample successfully (like configuring im_config with "joblocal" and/or "divlocal" or other graphics library name/path configurations)
- provide links to output or export results, where applicable
- document commands and options used to generate output or export results, where applicable
- instructions for placings local styles into desired Lstylelib, so they can be applied across multiple JOBs in customer's production environment

### Job Ticket/Library Considerations

Here are some considerations to make when sharing content. Following these guidelines will help ensure that others will be able to make use of your shared data.

- It is suggested, but not required, that any JOB specify std-fmt as the Style Library, noto as the Font Variant and noto as the Font Library in the job ticket
- JOB's style specs must all be local – if sample comes with mx spec, move its rules into local xx spec and clear mx spec field in job ticket
- It is encouraged to provide as clean as possible content, formatting commands, etc. so that all DIV(s) compose with little to no composition errors/warnings
- all sample JOB(s) demonstrating "output" or "export" functionalities should:
  - create output without errors/warnings to local file or directory
  - the "fully-operational" output result should be included within the JOB sample with appropriate link in the DIV_readme

### Graphics

In order to view graphics that are included with these sample jobs, you will need to make sure your Graphics Configuration is set correctly. To verify, do the following.
Launch the XPP Administrative Tools. From the Administrative Tools, click File -> Graphics Configuration. The Master Graphics Configuration Spec will open.

Create a new rule. Click Menu->Main Menu-> New Rule. In the Library Name field, type "graphics". In the Library Path field, type .. (two periods). This instructs XPP to look for a folder called
graphics in the current job directory. Store and exit from the Graphics Configuration, and you can also close the Administrative Tools application.

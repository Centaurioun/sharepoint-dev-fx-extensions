# Field Votes

## Summary

An extension that displays Vote counter and button to vote or unvote.
If the current user hasn't been voted, the button will become Vote button
but if the current user has been voted, it will become Unvote button.

The underlying value is an array of voter's login name in JSON format.

![picture of the extension in action](assets/preview.gif)

## Compatibility

![SPFx 1.15.2](https://img.shields.io/badge/SPFx-1.15.2-green.svg)
![Node.js v14 | v16](https://img.shields.io/badge/Node.js-v14%20%7C%20v16-green.svg)
![Compatible with SharePoint Online](https://img.shields.io/badge/SharePoint%20Online-Compatible-green.svg)
![Local Workbench Unsupported](https://img.shields.io/badge/Local%20Workbench-Unsupported-red.svg "Local workbench is no longer available as of SPFx 1.13 and above")


## Applies to

* [SharePoint Framework](https://docs.microsoft.com/sharepoint/dev/spfx/sharepoint-framework-overview)
* [Microsoft 365 tenant](https://docs.microsoft.com/sharepoint/dev/spfx/set-up-your-developer-tenant)


## Solution

Solution|Author(s)
--------|---------
react-field-votes | [Ari Gunawan](https://github.com/AriGunawan) ([@AriGunawan3023](https://twitter.com/arigunawan3023))

## Version history

Version|Date|Comments
-------|----|--------
1.2|October 18, 2022|Initial version

## Prerequisites

- Create a list that will have the vote button
- Create a new column: 
    - Internal Name: `SPFxVotes`
    - Display Name: Anything you want. e.g. Votes, Action, etc.
    - Type: `Multiple lines of text`
- My suggestion to prevent users manually update underlying votes data:
   - Disable `Edit in grid view` feature on the list view
      - Go to `List settings`
      - Go to `Advanced settings`
      - Disable quick edit
        ![disable quick edit](/assets/disable%20quick%20edit.png)
   - Remove `SPFxVotes` column from the form
     ![edit form](/assets/edit-form.gif)

## Minimal Path to Awesome

* Clone this repository
* in the command line run:
  * `npm install`
  * `gulp serve`

## Features

This extension illustrates the following concepts:

* Use [React](https://reactjs.org/) for displaying vote count on list view
* Use [React](https://reactjs.org/) for displaying vote/unvote button on list view
* Use [PnPJS](https://pnp.github.io/pnpjs/) for updating underlying data
* Use [SPFx Fast Serve](https://github.com/s-KaiNet/spfx-fast-serve) for increasing development productivity

## Debug URL for testing

Here's a debug URL for testing around this sample.

```
?debugManifestsFile=https://localhost:4321/temp/manifests.js&loadSPFX=true&fieldCustomizers={"SPFxVotes":{"id":"cfd41b03-0507-48c5-9fc8-e3dba6facfcd"}}
```


## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

## Help

We do not support samples, but we this community is always willing to help, and we want to improve these samples. We use GitHub to track issues, which makes it easy for  community members to volunteer their time and help resolve issues.

You can try looking at [issues related to this sample](https://github.com/pnp/sp-dev-fx-extensions/issues?q=label%3Areact-field-votes) to see if anybody else is having the same issues.

You can also try looking at [discussions related to this sample](https://github.com/pnp/sp-dev-fx-extensions/discussions?discussions_q=label%3Areact-field-votes) and see what the community is saying.

If you encounter any issues while using this sample, [create a new issue](https://github.com/pnp/sp-dev-fx-extensions/issues/new?assignees=&labels=Needs%3A+Triage+%3Amag%3A%2Ctype%3Abug-suspected&template=bug-report.yml&sample=react-field-votes&authors=@AriGunawan&title=react-field-votes%20-%20).

For questions regarding this sample, [create a new question](https://github.com/pnp/sp-dev-fx-extensions/issues/new?assignees=&labels=Needs%3A+Triage+%3Amag%3A%2Ctype%3Abug-suspected&template=question.yml&sample=react-field-votes&authors=@AriGunawan&title=react-field-votes%20-%20).

Finally, if you have an idea for improvement, [make a suggestion](https://github.com/pnp/sp-dev-fx-extensions/issues/new?assignees=&labels=Needs%3A+Triage+%3Amag%3A%2Ctype%3Abug-suspected&template=suggestion.yml&sample=react-field-votes&authors=@AriGunawan&title=react-field-votes%20-%20).

<img src="https://m365-visitor-stats.azurewebsites.net/sp-dev-fx-extensions/samples/react-field-votes" />
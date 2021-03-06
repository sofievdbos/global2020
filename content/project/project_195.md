{
  "Title": "Diffusion MRI brain masking (\"dwi2mask\")",
  "issue_number": 195,
  "link_to_issue": "https://github.com/ohbm/hackathon2020/issues/195",
  "labels": [
    {
      "name": "Apac hub",
      "description": "",
      "color": "90dee5"
    },
    {
      "name": "C / C++",
      "description": "some knowledge of C / C++ required",
      "color": "e0502c"
    },
    {
      "name": "Email ok",
      "description": "",
      "color": "bfdadc"
    },
    {
      "name": "FSL",
      "description": "some knowledge of FSL required",
      "color": "bfa0e8"
    },
    {
      "name": "Hackathon project",
      "description": "use this tag for submitted projects",
      "color": "fcffbc"
    },
    {
      "name": "dMRI",
      "description": "some knowledge of diffusion MRI required",
      "color": "996dff"
    },
    {
      "name": "git-1",
      "description": "can commit and push to a repository",
      "color": "44ff44"
    },
    {
      "name": "python",
      "description": "some knowledge of python required",
      "color": "fc8397"
    }
  ],
  "content": "## Project info\r\n\r\n**Title**: DWI brain masking\r\n\r\n**Project lead**: Robert E. Smith @Lestropie\r\n\r\n**[Timezone](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#timezone)**: UTC+10 (Australia east coast)\r\n\r\n**Hub**: Asia and Pacific\r\n\r\n**Description**:\r\n\r\nThe challenge of automatically extracting a brain mask from neuroimaging data has attracted a lot of interest in the context of high-resolution anatomical-contrast data. Processing pipelines involving Diffusion MRI data commonly also require derivation of a brain mask. This has however not attracted the same development interest, despite regular feedback that this is regularly a point of failure for group studies.\r\n\r\nThis project will involve development of a generalised interface for derivation of DWI brain masks in the [*MRtrix3* software](https://www.mrtrix.org/). The [current \"`dwi2mask`\" binary command](https://mrtrix.readthedocs.io/en/latest/reference/commands/dwi2mask.html#dwi2mask) (written in C++) will be replaced with an interface implemented in Python, through which the user will have the ability to select from a range of different algorithms available for performing these tasks. Alternative approaches for DWI brain masking implemented in other software packages will be wrapped in order to provide access to all of these alternatives within a standardised interface, integrating compatibility with all of the image formats supported by *MRtrix3*.\r\n\r\nIf successful, changes will be included in a future update to the *MRtrix3* software. [Contributors](https://github.com/MRtrix3/mrtrix3/blob/master/CONTRIBUTING.md) will be included in the built-in `git` [contribution statistics](https://github.com/MRtrix3/mrtrix3/graphs/contributors). We additionally credit contributors by showing their avatar at the bottom of the [*MRtrix3* website front page](https://www.mrtrix.org/), and in the changelog as reported on the community forum ([example](https://community.mrtrix.org/t/mrtrix-3-0-rc3-3-0-0-changelog/3552)). If there is [adequate test data](https://community.mrtrix.org/t/seeking-challenging-dwi-masking-data/3783) and differential performance between methods, a manuscript may be written reporting on the results of this analysis, on which all team members would be invited to contribute.\r\n\r\n**Link to project**: MRtrix3/mrtrix3#2075\r\n\r\n**Mattermost handle**: @lestropie\r\n\r\n**Goals for the OHBM Brainhack** / **Good first issues**:\r\n\r\nThe range of possible milestones are presented in MRtrix3/mrtrix3#2075. The minimum requirements for the Hackathon would be: Re-implementation of existing *MRtrix3* `dwi2mask` C++ code in Python; wrapper algorithm for executing FSL's `bet` tool on the mean *b*=0 image; have both of these approaches available from a common interface.\r\n\r\n**Skills**:\r\n\r\nSome experience with Python, *MRtrix3* and/or `git` would be advantageous; the pace of the project will however be tailored to the skillset of team members. No prior expectations are set on the quantity of team members.\r\n\r\nGood entry points for starting with the project would be:\r\n\r\n- Install *MRtrix3* [from source](https://mrtrix.readthedocs.io/en/latest/installation/build_from_source.html)\r\n\r\n- Install FSL\r\n\r\n- Take a look at the *MRtrix3* [demonstration script code](https://github.com/MRtrix3/MRtrix3_demo_code/blob/master/bin/demo_script), as presented in the [*MRtrix3* manuscript](https://www.sciencedirect.com/science/article/abs/pii/S1053811919307281).\r\n\r\n- Create a GitHub account if you have not done so already\r\n\r\n**Chat channel**: [hbmhack-dwi2mask](https://mattermost.brainhack.org/brainhack/channels/hbmhack-dwi2mask)\r\n\r\n**Video channel**:   https://us02web.zoom.us/j/6949814237  (password to be distributed via MatterMost)\r\n\r\n**Image for the OHBM brainhack website**:\r\n\r\n![Screenshot from 2020-06-14 10-48-08](https://user-images.githubusercontent.com/5637955/84582819-62f55880-ae34-11ea-8dc6-ffececea3e60.png)\r\n\r\n**Twitter-size summary**:\r\n\r\nDiffusion MRI brain masking (\"dwi2mask\")\r\nhttps://github.com/MRtrix3/mrtrix3/issues/2075\r\n@Lestropie\r\n#OHBMHackathon #Brainhack #OHBM2020\r\n\r\n## Project submission checklist\r\n*Once the issue is submitted, please check items in this list as you add under 'Additional project info'*\r\n\r\nPlease include the following above (all required):\r\n-   [x] Link to your project\r\n-   [x] Include your [Mattermost handle](https://mattermost.brainhack.org/) (i.e. your username).\r\n-   [x] Goals for the OHBM Brainhack: describe what you want to achieve during this brainhack. \r\n-   [x] Flesh out at least 2 \"good first issues\"\r\n-   [x] Skills: list skills that would be particularly suitable for your project. \r\n-   [x] Chat channel: A link to a chat channel that will be used during the OHBM Brainhack. \r\n-   [x] Video channel: Zoom personal meeting to be used; password to be made available at commencement of hackathon\r\n-   [x] Provide an image of your project for the OHBM brainhack website.\r\n\r\nYou can also include information about (all optional):\r\n-   [x] Number of participants, cf. [here](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#participant-capacity)\r\n-   [x] Twitter-size summary of your project pitch, cf. [here](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#twitter-size-summary-of-your-project-pitch)\r\n-   [ ] Set up a kanban board on your repository to better divide the work and keep track of things, cf [here](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#set-up-a-kanban-board)\r\n-   [x] Project snippet for the OHBM Brainhack website, cf. [here](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#project-snippet-for-the-ohbm-brainhack-website)\r\n\r\nWe would like to think about how you will credit and onboard new members to your project. We recommend reading references from [this section](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#credit-and-onboarding). If you'd like to share your thoughts with future project participants, you can include information about (recommended):\r\n-   [x] Specify how will you acknowledge contributions (e.g. listing members on a contributing page).\r\n-   [x] Provide links to onboarding documents if you have some.\r\n"
}
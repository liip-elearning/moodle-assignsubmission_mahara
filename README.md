# Mahara Assignment Submission Plugin

This repository houses an updated Mahara assignment submission plugin.

Developed for the University of Portland by Philip Cali and Tony Box (box@up.edu).

The original Moodle 1.9 version of these plugins were funded through a grant from the New Hampshire Department of Education to a collaborative group of the following New Hampshire school districts:

- Exeter Region Cooperative
- Windham
- Oyster River
- Farmington
- Newmarket
- Timberlane School District
  
The upgrade to Moodle 2.0 and 2.1 was written by Aaron Wells at Catalyst IT, and supported by:

- NetSpot
- Pukunui Technology

## Features

- XML-RPC integration with a Mahara installation
- Select portfolio
- If multiple submissions are allowed, it release a previously selected submission
- Abides by Moodle assignments config options
- Popup for quickly looking at submission (no windows... no tabs)

## Requirements

- Moodle 2.3+
- [Updated Mahara local plugin][1]
- [Mahara Feedback plugin][2] (Optional, but reccommended)

## Installation

Be sure that you have a version of Moodle that equal or greater than 2.2. Also make sure you have successfully
integrated your Moodle installation with a Mahara instance.

Mahara has detailed documenation on how to achieve that [on their wiki][3]. Once you have done that, you must
install the [updated Mhara local plugin][1] on your installation. Must then install this plugin one of two ways:

1. Download the source archive, and extract its contents on the following location `{Moodle_Root}/mod/assign/submission/mahara`
2. Execute the following command:

```
> git clone git@github.com:fellowapeman/assign-mahara.git {Moodle_Root}/mod/assign/submission/mahara
```

The remainder of the install is taken care of by Moodle by clicking on _Notifcations_.

## Feedback plugin

The only reason the feedback plugin exists is for properly releasing graded submissions in Mahara,
and Mahara outcomes. It's an optional install because its technically not required for a fully functional
Mahara assignment, but it's rcertainly reccommeded.

[1]: https://github.com/fellowapeman/local-mahara
[2]: https://github.com/fellowapeman/assign-mahara-feedback
[3]: https://wiki.mahara.org/index.php/System_Administrator's_Guide/Moodle//Mahara_Integration/View_Submission#Moodle_.26_Mahara_plugins_for_Portfolio_assignment_submission

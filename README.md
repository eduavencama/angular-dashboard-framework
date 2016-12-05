# “Problem identification and task identification” 
 
Eduard A. Avendaño Camacho, Cristian D. Gutierrez Gil, Carlos I. Zubieta León 
Universidad de los Andes, Bogotá, Colombia 
{ea.avendano, cd.gutierrez, ci.zubieta}@uniandes.edu.co 
Fecha de presentación: Octubre 4 de 2016 
  
## Business Comprehension:  
 
### About the company
 
AGZ is a multinational what work in the field of the construction and instalation of Industries projets.

### Direct Client
 
Our client is the PMO (Project Management Office). One of its main tasks is to present to the board of directors the progress of each of the projects compared to the baseline. 
 
### Identification of the problem 

In order to guarantee and control each of its projects the **PMO** must generate weekly and monthly reports from different departments to constantly verify the progress of the project and the administration of Money and Activities in each area.

These reports should be unified from different sources and formats of data that each department handles to be presented in a single format that is directed to the management area. Based on these unified final reports, management makes adjustments and restructuring decisions in each project, if necessary. This final format should be clear, understandable and should highlight the characteristics most relevant to the project.

Currently the process of **verification and unification of the sources is done by hand** through multiple tables of Excel, on the other hand, part of the information is processed by software called **Primavera** by **Oracle** that allows the administration and control of multiple projects, for this case, the benefit provided by the tool is not relevant, because the client **does not handle multiple projects at the same time**. Primavera also generates a kind of dashboard that is **very restrictive in terms of displaying the parameters of interest of the client**. 

The client has been working on improving the process of generating the reports of:
- Activity and Performance.
- Costs. 
 
For this purpose, it has been working with multiple departments and with management to determine the relevant data and the presentation of the data for each of the reports. Thanks to this work we achieved a dashboard of **activity and performance** debugged with only the parameters of interest to the company. For this dashbord the client needs to improve the way of presentation and navigation, as currently **must spend time in the generation of the dashboard whenever it requires generating the weekly and monthly report for each project**.

On the Cost dashboard the client is in the process of debugging and coordination between departments and management. **At the moment they have a base of the board of costs that is not definitive**, reason why they require a proposal to represent the costs that implies each project.  In addition, he told us that with the current process it takes a lot of effort and time **to detect deviations of time and money in the execution of each one of the projects**.
 
## Characterization of the Data 
### What 
The dataset is type **table** (All tables are in an Excel workbook that was obtained from the "Spring" program).
As for the **attributes**, most are of a sequential quantitative type. But there are also some with a special semantics (use a temporal semantics), which are used to identify a date (day, month and year). 
 
### Why 

Several sections of interest were identified: Earned value , man hours and productivity:

#### Earned Value 
- **T1.** *Identify* what are the deviations in * the areas * that most influence the performance of the project.
- **T2.** *Compare* PV *, * EV * and * AC * distribution for the areas of interest in the project.
- **T3.** *Identify* in a specific week the values for * PV *, * EV * and * AC *.
 
#### Man Hours 
- **T4.** *Present* what are the hours consumed both directly and indirectly in the project by the people.
- **T5.** *Compare* Scheduled Man Hours with Reals for each period.
 
#### Productivity

- **T6.** *Compare* the planned distribution of the most relevant parameters in the project (Concrete, Steel, Structure, Welding) vs actual distribution. 
- **T7.** *Present* the distribution of the multiple parameters of expected vs. actual production.
 
### How 
  
Activity and Performance Dashboard
 
#### Earned Value 
 
The marks used are the horizontal and vertical position lines, which have the color channel to identify the EV, PV and AC. 
 
**T1, T2 y T3**: For these tasks a "MulticharLine" is used where the axis ** x ** represents the dates with intervals of weekly cut periods, in the axis ** and ** the number of hours of the Planned Value, Value gained and Current Cost, for these categories the channel hue is used to identify them among themselves.  

<p align="center"> 
<img src="https://cloud.githubusercontent.com/assets/13947710/19095498/86aa1b54-8a5b-11e6-97cd-985011271fbf.png">  
<br>

# angular-dashboard-framework

[![Packagist](https://img.shields.io/packagist/l/doctrine/orm.svg)](https://github.com/angular-dashboard-framework/angular-dashboard-framework/blob/master/LICENSE.md) [![Build Status](https://travis-ci.org/angular-dashboard-framework/angular-dashboard-framework.svg?branch=master)](https://travis-ci.org/angular-dashboard-framework/angular-dashboard-framework) [![Coverage Status](https://coveralls.io/repos/angular-dashboard-framework/angular-dashboard-framework/badge.svg?branch=master&service=github)](https://coveralls.io/github/angular-dashboard-framework/angular-dashboard-framework?branch=master) [![Dependency Status](https://www.versioneye.com/user/projects/562008b836d0ab001900070b/badge.svg?style=flat)](https://www.versioneye.com/user/projects/562008b836d0ab001900070b) [![Join the chat at https://gitter.im/sdorra/angular-dashboard-framework](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/angular-dashboard-framework/angular-dashboard-framework?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

> Dashboard framework with Angular.js and Twitter Bootstrap.

The api of angular-dashboard-framework (adf) is documented [here](http://angular-dashboard-framework.github.io/angular-dashboard-framework/docs/). A getting
started guide can be found [here](https://github.com/angular-dashboard-framework/angular-dashboard-framework/wiki/Getting-started).
Follow me ([@ssdorra](https://twitter.com/ssdorra)) on twitter for latest updates and news about adf.

## Demo

A live demo of the adf can be viewed [here](http://angular-dashboard-framework.github.io/angular-dashboard-framework/). The demo uses html5 localStorage to store the state of the dashboard. The source of the demo can be found [here](https://github.com/angular-dashboard-framework/angular-dashboard-framework/tree/master/sample).

A more dynamic example can be found [here](https://github.com/angular-dashboard-framework/adf-dynamic-example).

## Build from source

Install bower and gulp:

```bash
npm install -g bower
npm install -g gulp
```

Clone the repository:

```bash
git clone https://github.com/angular-dashboard-framework/angular-dashboard-framework
cd angular-dashboard-framework
```

Install dependencies:

```bash
npm install
bower install
```

Checkout git submodule widgets:

```bash
git submodule init
git submodule update
```

You can start the sample dashboard, by using the serve gulp task:

```bash
gulp serve
```

Now you open the sample in your browser at http://localhost:9001/sample

Or you can create a release build of angular-dashboard-framework and the samples:

```bash
gulp all
```
The sample and the final build of angular-dashboard-framework are now in the dist directory.


## Contributing

Please do not commit changes to the dist folder. The dist folder is only generated for releases.


## License

    The MIT License

    Copyright (c) 2015, Sebastian Sdorra

    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be included in
    all copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.

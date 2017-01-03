---
layout: default
---
# Technical Skills

| Standard Languages         | Web Development                                          |  IDE's and Tools         | Scripting Languages | Mobile Development |
|:---------------------------|:---------------------------------------------------------|:-------------------------|:--------------------|:-------------------|
| Java                       | HTML                                                     | Eclipse                  | Python              | Android Development|
| C                          | CSS                                                      | XCode                    | Perl                | iOS Development    |             
| C++                        | LAMP Stack (Linux, Apache, MySQL and PHP/Python/Perl)    | Visual Studio            | Bash                | MacOS Development  |
| C#                         | MEAN Stack (MongoDB, ExpressJS, AngularJS, and Node.js)  | Spring Tool Suite        | Ruby                |                    |
| Objective C                | MeteorJS                                                 | Atom                     | Markdown            |                    |
| Swift                      | ASP.NET MVC                                              | Amazon AWS               |                     |                    |
| Spring Boot                |                                                          | Digital Ocean Servers    |                     |                    |

* * *

# Work Experience

### Avidxchange: Software Development Intern (2016)
- Researched, designed, and built a prototype IVR automation solution using a C# ASP.Net MVC application, Twilio Cloud API, and Authy Cloud API
- Developed a two factor authentication system
- Designed and built a web automation framework using C# and Selenium
- Built a Node.js and MongoDB website for testing bill payment automation systems

### Center for Digital Humanities: System Administration & Software Development (2016)
- Responsible for maintaining and backing up development and production servers
- Implemented source control, virtual private servers, and Docker containers
- Worked on Meteor.js application for touchscreen displays in USC Museum

### Perahealth: Software Development Intern (2015)
- In an Agile Development process, drastically overhauled an AngularJS web application with the Highcharts charting library and a SQL database
- Fixed Javascript and AngularJS bugs in several projects
- Created a Java program to simulate data feeds for testing software
- Created an iOS application with a Java data api to access a SQL database

### 3D Systems: Quality Assurance Intern (2013 – 2014)
- Responsible for testing software and firmware for 3D Printers
- Helped create and implement testing plans for printer software and firmware
- Created an automated GUI testing system using Sikuli
- Assisted developers in fixing minor bugs using C# and XAML

* * *

# Education
### College
- University of South Carolina
- Expected graduation date: Spring 2018
- Major: Computer Science

### High school
- Homeschooled
- Graduated Spring 2014
- Dual Enrollment College - High school 2012 - 2014
  - York Technical College
  - Grand Caynon University (Online)
  - San Jose State University (Online)

* * *

# Side Projects
Since I was around 11 or 12 years old I have been interested in programming and software development. The best way to learn a new programming language or technique is to do a few tutorials or build a side project with that language or technology. Over the years many I have built many side projects and most of them consisted of following tutorials. Listed below are the details for a few of the bigger and more interesting projects that I have completed.

## MEIRLBOT
- Source Code: [GitHub](https://github.com/tmoon8730/meirlbot.git)
- Description: The MEIRLBOT is a set of Java Spring Boot applications for the purpose of creating and displaying memes. The main reason for creating this project was to learn new technologies and build resumes.
- Technical Spec: Java Spring Boot Application
- Code Example:

``` java
@SpringBootApplication
public class MemeExchangeApplication {

  public static void main(String[] args) {
    SpringApplication.run(MemeExchangeApplication.class, args);
  }
}
```

- Screenshot: ![](/assets/images/meirlbot-screenshot.png)

## Nutriments
- Website: [http://nutrimentsapp.com/](http://nutrimentsapp.com/)
- Source Code: [GitHub](https://github.com/tmoon8730/FATStats)
- Description: Nutriments is an iOS Application for simple and quick exercise and supplement tracking
- Technical Spec: iOS Application developed in Swift
- Code Example:

``` swift
func createDrive(managedContext: NSManagedObjectContext, quarter: String, time: String, yardLine: String) -> Bool{
    let entityDrive = NSEntityDescription.entityForName("DriveEntity", inManagedObjectContext: managedContext)
    let newDrive = DriveEntity(entity: entityDrive!, insertIntoManagedObjectContext: managedContext)
    newDrive.quarter = quarter
    newDrive.time = time
    newDrive.yardLine = yardLine
    do{
        try newDrive.managedObjectContext?.save()
        print("New drive added: \(newDrive.quarter!) with \(newDrive.time!) left on the \(newDrive.yardLine!) yard line")
        return true
    }catch{
        let saveError = error as NSError
        print(saveError)
    }
    return false
}
```

- Screenshot:

![](http://nutrimentsapp.com/img/portfolio/buttonsSupplements.jpg)


## AndroidMultiTool
- Source Code: [GitHub](https://github.com/tmoon8730/androidmultitool)
- Description: A Android Application with a slew of different useful tools including:
  - Alarm Clock
  - Custom Web Browser
  - Email App
  - Present Fortune Teller
  - A Database Access Object
- Technical Spec: Java Application developed in Java
- Code Example:

``` java
@Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_alarm_manager);
        Toolbar toolbar = (Toolbar) findViewById(R.id.toolbar);
        setSupportActionBar(toolbar);

        alarm = new AlarmManagerBroadcastReceiver();

        FloatingActionButton fab = (FloatingActionButton) findViewById(R.id.fab);
        fab.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Snackbar.make(view, "Replace with your own action", Snackbar.LENGTH_LONG)
                        .setAction("Action", null).show();
            }
        });
    }
```

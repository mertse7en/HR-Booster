
# Job Boosty

Job Boosty is a comprehensive tool designed to streamline the job search process for both Human Resources professionals and job seekers. It offers two main functionalities: HR Booster and Job Finder Booster.

## 1- HR Booster

The HR Booster component of Job Boosty is tailored for Human Resources professionals. This feature automates the process of analyzing job descriptions and candidates, providing an efficient solution for candidate selection. 

HR Booster is a tool designed to facilitate HR professionals in matching job descriptions with potential candidates available on LinkedIn. It takes inputs in a specific format for job descriptions and a list of LinkedIn profiles, and generates an output table displaying the similarity scores between the job description and the LinkedIn profiles.

### Example

### HR - Input1: Job Description
---

To use the tool, input the job description following a specific format:

```

Responsibilities:

Software Development, Participating in scrum events, Product Demonstration to the customers.
Development and operation of the framework for generating reference data for labelling algorithms in the form of KPIs (lane markings, obstacles, the lane area travelled over and the trajectory travelled). These must be adapted to both to local and the cloud infrastructure. The goal is to increase the accuracy in order to minimize the effort for manual corrections.

Mandatory Skills Description:
Python (including interaction with cloud, networking, authentication management)
Strong AWS experience: migration of apps to AWS platform (lambdas, VPC, jumphosts, IAM roles, EMR)
Container services (Docker, AWS EKS, Kubernetes/OpenShift)
Data Processing: Apache Spark, Pandas
CI/CD, git

Working experience in a big company for the last 2 years (no freelance or freelancer based companies like 5-10 ppl or companies that look like not real w/o website, easily available info about organization in the internet).

Nice-to-Have Skills:
Orchestration (Apache Airflow / Step function)
Infrastructure as Code (Terraform / AWS CloudFormation)
Databases (SQL / NoSQL - DynamoDB / Redshift / RDS ...)
Automotive data formats (SOME/IP, non-verbose DLTs, FIBEX, etc.)
Dashboard systems (Kibana, Grafana, ...)
Scala
```



### HR - Input2: LinkedIn Profiles
---


Provide the LinkedIn profile URLs in a list format:

1. (https://www.linkedin.com/in/mert-seven-439935149/)
2. (https://www.linkedin.com/in/jane-doe-123456789/)
3. (https://www.linkedin.com/in/john-smith-987654321/)
4. (https://www.linkedin.com/in/emma-johnson-567890123/)
5. (https://www.linkedin.com/in/david-miller-345678901/)
6. (https://www.linkedin.com/in/sarah-wilson-789012345/)
7. ....

## Output

Upon inputting the job description and LinkedIn profiles, HR will receive an output table displaying candidate names, profile links, and similarity scores:

| Name  | Link                                               | Similarity Score |
|-------|----------------------------------------------------|------------------|
| Jane  | https://www.linkedin.com/in/jane-doe-123456789/    | 9.27             |
| John  | https://www.linkedin.com/in/john-smith-987654321/  | 5.23             |
| Emma  | https://www.linkedin.com/in/emma-johnson-567890123/| 4.23             |
| David | https://www.linkedin.com/in/david-miller-345678901/| 3.42             |
| Sarah | https://www.linkedin.com/in/sarah-wilson-789012345/| 9.72             |

Based on the similarity scores, Jane and Sarah could be suitable candidates for the job.





## 2-Job Finder Booster

## Description

Job Finder Booster is a tool designed to assist job seekers in finding suitable job descriptions based on their resumes. It takes inputs such as the job seeker's resume details including skills and experience, specified role names, country preferences, working type, and relocation preferences to provide a list of potential job descriptions that match the criteria.

## Inputs

### Resume Example

The job finder will input their resume details in the specific format!

Dummy format:


Experience: 3 years
Python, AWS, Airflow, Docker, K8s etc.




### Seeking Role Name and Preferences

Specify the role name(s) and preferences:

- Role Name: Data Engineer, Data Scientist
- Country: Switzerland
- Working Type: Remote, Hybrid, Unknown
- Relocation: Yes, No, Unknown

## Output

Upon providing the resume details and preferences, the job finder will receive an output table displaying potential job descriptions that match their criteria:

| Link                                  | Similarity Score | Experience Needed | Working Type | Relocation |
|---------------------------------------|------------------|-------------------|--------------|------------|
| https://www.linkedin.com/jobs-id1     | 8.3              | 3 years           | Remote       | Yes        |
| https://www.linkedin.com/jobs-id12312 | 4.0              | 6 years           | Hybrid       | No         |
| https://www.linkedin.com/jobs-id321   | 7.8              | 2 years           | Unknown      | Unknown    |
| https://www.linkedin.com/jobs-id456   | 6.5              | 4 years           | Remote       | Yes        |
| https://www.linkedin.com/jobs-id789   | 5.2              | 5 years           | Hybrid       | Unknown    |

The output provides LinkedIn job links, similarity scores, required experience, working type, and relocation details for potential job descriptions. Job seekers can use this information to explore and apply for relevant job opportunities.

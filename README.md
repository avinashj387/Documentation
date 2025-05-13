# API Documentation

## Table of Contents
1. [My Courses](#my-courses)
   - 1.1 [Get Paginated Courses](#1-get-paginated-courses)
   - 1.2 [Get Course Module](#2-get-course-module)
   - 1.3 [Get To-Do List](#3-get-to-do-list)
   - 1.4 [Get My Courses](#20-get-my-courses)

2. [Leaderboard](#leaderboard)
   - 2.1 [Get User Rankings](#4-get-user-rankings)
   - 2.2 [Get Category Rankings](#5-get-category-rankings)

3. [Explore](#explore)
   - 3.1 [Get All Categories](#6-get-all-categories)
   - 3.2 [Get Subcategories](#7-get-subcategories)
   - 3.3 [Get Category Courses](#8-get-category-courses)

4. [Knowledge Library](#knowledge-library)
   - 4.1 [Get News Updates](#9-get-news-updates)
   - 4.2 [Get Quiz Corner](#11-get-quiz-corner)
   - 4.3 [Get Survey Corner](#12-get-survey-corner)
   - 4.4 [Get Polls Corner](#14-get-polls-corner)

5. [Media Library](#media-library)
   - 5.1 [Get Media Albums](#10-get-media-library)

6. [Central Library](#central-library)
   - 6.1 [Get Book Categories](#17-get-central-book-library-categories)

7. [Publication Library](#publication-library)
   - 7.1 [Get Publications by Folder](#15-get-publications-by-folder)
   - 7.2 [Get Social File](#16-get-social-file)
   - 7.3 [Get Policy Document](#19-get-policy-document)
8. [Catalog](#catalog)
   - 8.1 [Get My Courses](#81-get-my-courses)
   - 8.2 [Get Course Count](#82-get-course-count)
   - 8.3 [Get Selected Languages](#83-get-selected-languages)
   - 8.4 [Get Course Enrollment Config](#84-get-course-enrollment-config)
   - 8.5 [Get All Categories](#85-get-all-categories)
  
- [Edit Course](#edit-course)

   - 8.6 [Subset of Subcategories](#subset-of-subcategories)



      * [1. Get All Categories](#1get-all-categories)
      * [2. Get Subcategories by Category](#2get-subcategories-by-category)
      * [3. Create a SubSubCategory (Subset)](#3create-a-subsubcategory-subset)
      * [4. List All SubSubCategories](#4list-all-subsubcategories)
      * [5. Get Total SubSubCategory Count](#5get-total-subsubcategory-count)

9. [Competency](#competency)
    - 9.1 [Get Competency Hub Data](#91-get-competency-hub-data)
    - 9.2 [Get Competency Spider Chart](#92-get-competency-spider-chart)
      
10. [Calendar](#calendar)
    - 10.1 [Get Date Format](#101-get-date-format)
    - 10.2 [Get ILT Calendar Data](#102-get-ilt-calendar-data)
    - 10.3 [Check Batch Nomination Status](#103-check-batch-nomination-status)
    - 10.4 [Get Calendar Help Info](#104-get-calendar-help-info)
    - 10.5 [Get Academy List](#105-get-academy-list)
    - 10.6 [Get Organization Calendar](#106-get-organization-calendar)
    - 10.7 [Export ILT Calendar](#107-export-ilt-calendar)
    - 10.8 [Export Trainer Calendar](#108-export-trainer-calendar)
    - 10.9 [Get Schedule Data](#109-get-schedule-data)
    - 10.10 [Get Schedule Count](#1010-get-schedule-count)
    - 10.11 [Check Past Schedule Cancellation](#1011-check-past-schedule-cancellation)
    - 10.12 [Get Localization Strings](#1012-get-localization-strings)
    - 10.13 [Get Nomination Data](#1013-get-nomination-data)
    - 10.14 [Get Nomination Count](#1014-get-nomination-count)
    - 10.15 [Get Training Attendance](#1015-get-training-attendance)
      
11. [Profile](#profile)
    - 11.1 [Get Encrypted User ID](#111-get-encrypted-user-id)
    - 11.2 [Get Profile Permissions](#112-get-profile-permissions)
    - 11.3 [Get User Configurable Parameters](#113-get-user-configurable-parameters)
    - 11.4 [Check Federation ID Status](#114-check-federation-id-status)
    - 11.5 [Get User Profile](#115-get-user-profile)
    - 11.6 [Get User Settings](#116-get-user-settings)
    - 11.7 [Get Profile Picture](#117-get-profile-picture)
    - 11.8 [Get User Details by ID](#118-get-user-details-by-id)
    - 11.9 [Get Competency Status Report](#119-get-competency-status-report)
    - 11.10 [Get Key Area Settings Count](#1110-get-key-area-settings-count)
    - 11.11 [Get Key Area Settings](#1111-get-key-area-settings)
    - 11.12 [Check External Certificate Status](#1112-check-external-certificate-status)
    - 11.13 [Get User Certificates](#1113-get-user-certificates)
    - 11.14 [Get User Certificates Count](#1114-get-user-certificates-count)
    - 11.15 [Check VIMEO Status](#1115-check-vimeo-status)
    -  [11.16 Upload Profile Picture](#1116-upload-profile-picture)
    -  [11.17 Get Profile Picture Size Limit](#1117-get-profile-picture-size-limit)
12. [Course Management](#course-management)
    - 12.1 [Get LCMS Media](#121-get-lcms-media)
    - 12.2 [Get File Format Size](#122-get-file-format-size)
    - 12.3 [Get Media Count](#123-get-media-count)
    - 12.4 [Upload SCORM Content](#124-upload-scorm-content)
    - 12.5 [Upload PDF Content](#125-upload-pdf-content)
    - 12.6 [Content Size Limits](#126-content-size-limits)
    - 12.7 [H5P Content](#127-h5p-content)
    - 12.8 [Video Content](#128-video-content)
    - 12.9 [Survey Content](#129-survey-content)
    - 12.10 [Audio/Podcast](#1210-audiopodcast)
    - 12.11 [YouTube Integration](#1211-youtube-integration)
    - 12.12 [External Links](#1212-external-links)
    - 12.13 [Assignments](#1213-assignments)
   - [Edit Course](#edit-course)

13. [Module Management](#module-management)
    - 13.1 [Get Module Data](#131-get-module-data)
    - 13.2 [Get Media Count](#132-get-media-count)
    - 13.3 [Search LCMS Media](#133-search-lcms-media)
      
14. [Assessment Attempt Management](#14-assessment-attempt-management)

* [14.1 Get All Assessment Attempts](#1-get-all-assessment-attempts)
* [14.2 Get Assessment Attempt Count](#2-get-assessment-attempt-count)
* [14.3 Get Modules for Assessment Course](#3-get-modules-for-assessment-course)
* [14.4 Search Active or Inactive User](#4-search-active-or-inactive-user)
* [14.5 Add Assessment Attempt](#5-add-assessment-attempt)
* [14.6 Upload Attempt File](#6-upload-attempt-file)
* [14.7 Download Template File](#7-download-template-file)
* [14.8 Save Uploaded File Data](#8-save-uploaded-file-data)
15. [MicroLearning](#15-microlearning)
- [15.1 Get MicroLearning List](#1-get-microlearning-list-paginated)
- [15.2 Get MicroLearning Count](#2-get-microlearning-count)
- [15.3 Create MicroLearning Module](#3-create-microlearning-module)
- [15.4 Get MicroLearning Details by ID](#4-get-microlearning-details-by-id)
- [15.5 Get Page Number for MicroLearning](#5-get-page-number-for-microlearning)
16. [Assessment Report APIs](#16-assessment-report-apis)
- [16.1 Get Configurable Report Parameters](#1-get-configurable-report-parameters)
- [16.2 Get Course Data](#2-get-course-data)
- [16.3 Get Assessment Result Sheet](#3-get-assessment-result-sheet)
- [16.4 Get Assessment Result Count](#4-get-assessment-result-count)
- [16.5 Get Assessment Result Graph Data](#5-get-assessment-result-graph-data)
- [16.6 Export Assessment Result Sheet](#6-export-assessment-result-sheet)
  
 17. [Additional Assessment Report APIs](#17-additional-assessment-report-apis)
- [17.1 Get Failed Assessment Result Sheet](#1-get-failed-assessment-result-sheet)
- [17.2 Get User Assessment Sheet](#2-get-user-assessment-sheet)
- [17.3 Get User Assessment Sheet Count](#3-get-user-assessment-sheet-count)
- [17.4 Get Assessment Response Analysis](#4-get-assessment-response-analysis)
 18. [Assessment Response Analysis Report](#18-assessment-response-analysis-report)
- [18.1 Get Assessment Response Analysis](#1-get-assessment-response-analysis)

 19. [Assessment Reports](#19-assessment-reports)
- [19.1 Get Top 5 Performers Export](#1-get-top-5-performers-export)
- [19.2 Get Top Performer Graph](#2-get-top-performer-graph)
- [19.3 Get Bottom 5 Performers Export](#3-get-bottom-5-performers-export)
- [19.4 Get Unit-wise Assessment Report Export](#4-get-unit-wise-assessment-report-export)
- [19.5 Get Unit-wise Assessment Graph](#5-get-unit-wise-assessment-graph)
- [19.6 Get Course Completion Rate Export](#6-get-course-completion-rate-export)
- [19.7 Get Course Completion Rate Data](#7-get-course-completion-rate-data)
- [19.8 Get Categories](#8-get-categories-for-filters)
- [19.9 Get Category-wise Report Export](#9-get-category-wise-report-export)
- [19.10 Get Category-wise Report Graph](#10-get-category-wise-report-graph)
- [19.11 Get Deployed vs Completed Assessment Report Export](#11-get-deployed-vs-completed-assessment-report-export)
- [19.12 Get Deployed vs Completed Assessment Graph](#12-get-deployed-vs-completed-assessment-graph)

 20. [ILT and Attendance Reports](#20-ilt-and-attendance-reports)
- [20.1 ILT Completion Report](#1-ilt-completion-report)
- [20.2 ILT Consolidated Report](#2-ilt-consolidated-report)
- [20.3 Learning Report (Search by Course)](#3-learning-report-search-by-course-name)
- [20.4 Export Learning Report](#4-export-learning-report-wns-report)
- [20.5 Export Schedule-wise Attendance Report](#5-export-schedule-wise-attendance-report)
- [20.6 Get Schedule-wise Attendance Report](#6-get-schedule-wise-attendance-report)
- [20.7 Get Schedule-wise Attendance Report Count](#7-get-schedule-wise-attendance-report-count)
- [20.8 Export Attendance Summary Report](#8-export-attendance-summary-report)
- [20.9 Get Attendance Summary Report](#9-get-attendance-summary-report)
- [20.10 Get Attendance Summary Report Count](#10-get-attendance-summary-report-count)
 [Internal Trainers Schedule Report](#21-internal-trainers-schedule-report)
- [20.11 Search for Internal Trainers](#1-search-for-internal-trainers)
- [20.12 Export Internal Trainers Schedule Report](#2-export-internal-trainers-schedule-report)
21. [Performance & Competency Management](#21-performance--competency-management)
    - 21.1 [Job Profiles Management](#211-job-profiles-management)
    - 21.2 [Career Roadmap Management](#212-career-roadmap-management)
    - 21.3 [Competencies Dictionary](#213-competencies-dictionary)
    - 21.4 [Competency Review Parameters](#214-competency-review-parameters)
    - 21.5 [Job Description Management](#215-job-description-management)
    - 21.6 [Competency Import/Export](#216-competency-importexport)

22. [Internal Trainers Schedule Report](#22-internal-trainers-schedule-report)
    - 22.1 [Search for Internal Trainers](#221-search-for-internal-trainers)

## My Courses

### 1. Get Paginated Courses
- **Endpoint**: `GET /api/v1/mycourses/{pageNumber}/{pageSize}/`
- **URL**: `https://gogetempowered.com/api/v1/mycourses/{pageNumber}/{pageSize}/`
- **Authentication**: Bearer Token
- **Parameters**:
  - `pageNumber`: Integer (1-based index)
  - `pageSize`: Integer (items per page)
- **Response**: Array of course objects
```json
[
  {
    "courseId": 28686,
    "title": "Courseassignment1",
    "mission": null,
    "description": "",
    "thumbnailPath": "../../../assets/img/Thumbnail_vectors/img_thumb96.jpg",
    "categoryName": "",
    "subCategoryName": null,
    "subSubCategoryName": null,
    "code": "10790",
    "courseFee": 0.0,
    "currency": "",
    "courseType": "elearning",
    "completionPeriodDays": -1,
    "courseCreationdDays": 3,
    "numberofModules": 1,
    "categoryId": null,
    "subCategoryId": null,
    "subSubCategoryId": null,
    "courseRating": 0.0,
    "status": "completed",
    "isFeedback": false,
    "isAssignment": false,
    "isAssessment": false,
    "isPreAssessment": false,
    "isCertificateIssued": false,
    "courseStartDate": "2025-05-04T12:53:05",
    "courseCompleteDate": "2025-05-07T12:53:05",
    "createdDate": null,
    "assignDate": null,
    "rewardPoint": null,
    "isCourseApplicable": true,
    "courseApprovalStatus": "Enrolled",
    "competencyCategory": null,
    "competencyCategoryID": 0,
    "assessmentPercentage": "--",
    "scheduleRequestStatus": "",
    "durationInMinutes": 0,
    "assessmentResult": "--",
    "isPreRequisiteCourse": false,
    "isExternalProvider": false,
    "externalProvider": null,
    "courseURL": null,
    "isRetraining": false,
    "nodalApprovalStatus": "Not Requested",
    "isSCORM": false,
    "firstAccessDate": null,
    "lastAccessDate": null,
    "timeSpent": null,
    "views": 0,
    "progressinpercentage": 0,
    "score": 0,
    "assignmentType": "",
    "courseDueDate": "NA",
    "pathLink": null,
    "alreadyEnrolled": null,
    "totalRating": null,
    "externalDescription": null
  }
]
```

### 2. Get Course Module
- **Endpoint**: `GET /api/v1/mycourses/Getmodule/{courseId}`
- **URL**: `https://go-getempowered.com/api/v1/mycourses/Getmodule/{courseId}`
- **Authentication**: Bearer Token
- **Response**: Detailed course module information
```json
{
  "courseId": 14883,
  "courseType": "elearning",
  "courseCode": "6144",
  "categoryName": "",
  "courseTitle": "new deployment testing",
  "numberofModules": 1,
  "completionPeriodDays": -1,
  "courseFee": 0.0,
  "currency": "",
  "thumbnailPath": "/assets/img/Thumbnail_vectors/img_thumb86.jpg",
  "description": "",
  "learningApproach": false,
  "language": "",
  "courseCreditPoints": 0.0,
  "preAssessmentId": 0,
  "assessmentId": 0,
  "feedbackId": 0,
  "isFeedbackOptional": false,
  "assignmentId": 0,
  "isPreAssessment": false,
  "isAssessment": false,
  "isFeedback": false,
  "isAssignment": false,
  "isCertificateIssued": false,
  "status": "completed",
  "assessmentStatus": "incompleted",
  "preAssessmentStatus": "",
  "feedbackStatus": null,
  "contentStatus": "completed",
  "adminName": "LMS Admin",
  "courseRating": 0.0,
  "courseRatingCount": 0,
  "isAdaptiveLearning": false,
  "progressPercentage": 100,
  "duration": 0,
  "courseAssignedDate": "5/9/2025 12:43:48 PM",
  "lastActivityDate": "3/29/2024 10:36:44 AM",
  "isDilinkingILT": false,
  "assignmentStatus": "",
  "isModuleHasAssFeed": true,
  "isManagerEvaluation": false,
  "managerEvaluationStatus": "NA",
  "isPreRequisiteCourse": false,
  "modules": [
    {
      "moduleId": 14180,
      "moduleName": "External link",
      "mimeType": "",
      "isSecuredContent": false,
      "path": "t5aPAKTyAwf3Nw6CcugNrHZWnaJcijMdzqR7yGFkF+nlB6FaPgG2hwvN6DTeeMFEiuARHoIe3QDLf2e+Np6DcfjtGqDyh8wC1fnf6YIoFWhdzDi10ZXBzmlfSUACMYhH9/CERJNbbiBVXovLk9zuxlkgkNFdDMxTaWhFaxd9DytE7PKSp2eruaUzbI/t3U/B5KjAWzuQYAuIOAhnUOMEmKtgGY5Er4/qiqtIsRYIcB2FmNwQUHtuhR8xrSh14yt7lVDAQInSyLyuW+0KAmvBD26VtlKaOntgSSQ/y6PD2wA=",
      "zipPath": "",
      "moduleType": "externalLink",
      "actualModuleType": null,
      "thumbnail": "",
      "description": "External link",
      "assesmentType": null,
      "isLearnerFeedback": false,
      "isTrainerFeedback": false,
      "isMobileCompatible": true,
      "duration": 0.0,
      "creditPoints": 0,
      "preAssessmentId": 0,
      "assessmentId": 0,
      "feedbackId": 0,
      "lcmsId": 11867,
      "youtubeVideoId": "",
      "externalLCMSId": null,
      "isPreAssessment": false,
      "isAssessment": false,
      "isFeedback": false,
      "status": "completed",
      "assessmentStatus": null,
      "preAssessmentStatus": null,
      "feedbackStatus": null,
      "contentStatus": "completed",
      "sectionId": null,
      "batchId": 0,
      "batchCode": "",
      "batchName": "",
      "scheduleID": 0,
      "scheduleCode": "",
      "startDate": null,
      "endDate": null,
      "registrationEndDate": null,
      "startTime": null,
      "endTime": null,
      "placeName": "",
      "city": "",
      "address": "",
      "trainingRequestStatus": "",
      "sequenceNo": 2,
      "location": "",
      "finalDate": "",
      "completionPeriodDays": 0,
      "isEnableModule": true,
      "activityID": null,
      "isMultilingual": false,
      "selectedLanguageCode": "en",
      "isEmbed": true,
      "bbBmeetingDetails": [],
      "apizooms": null,
      "apiteams": null,
      "apigsuit": null,
      "attendanceStatus": "",
      "waiverStatus": "ATTENDANCE",
      "scheduleCreatedBy": 0,
      "tz_StartDt": "0001-01-01T00:00:00",
      "tz_EndDt": "0001-01-01T00:00:00",
      "academyAgencyName": "",
      "feedbackRating": null,
      "trainerName": null,
      "scheduleFeedbackId": null,
      "scheduleFeedbackStatus": null,
      "assignmentId": 0,
      "isAssignment": false,
      "assignmentStatus": ""
    }
  ],
  "isShowViewBatches": false,
  "expiryMessage": null,
  "isCourseExpired": null,
  "externalProvider": null,
  "externalProviderCategory": null,
  "isOJT": false,
  "ojtStatus": "NA",
  "ojtId": 0,
  "isVisibleAssessmentDetails": true,
  "startDate": "",
  "endDate": "",
  "retrainingDate": "NA",
  "assignmentType": "",
  "feedbackRating": null,
  "aasectId": 0,
  "isANCC": false,
  "faqPath": ""
}
```


### 3. Get To-Do List
- **Endpoint**: `GET /api/v1/ToDoPriorityList/GetToDoList`
- **URL**: `https://gogetempowered.com/api/v1/ToDoPriorityList/GetToDoList`
- **Authentication**: Bearer Token
- **Response**: Array of to-do items
```json
[
  {
    "id": 14,
    "title": "Critical Thinking",
    "scheduleDate": "06 Jan 2025",
    "endDate": "30 Nov 2025",
    "priority": true,
    "status": "completed",
    "type": "Course",
    "moduleType": "MultiModule",
    "assignmentType": ""
  }
]
```

---

## Leaderboard

### 4. Get User Rankings
- **Endpoint**: `POST /api/v1/User/GetRanking`
- **URL**: `https://gogetempowered.com/api/v1/User/GetRanking`
- **Authentication**: Bearer Token
- **Payload**: 
  ```json
  {"ranks":10,"configuredColumnName":"undefined","houseCode":null}
```json
{
  "topRanking": [
    {
      "userId": 0,
      "euSerId": "fk2zuGnuQ/lJ2By+PLvNTg==",
      "userName": "LMS Admin",
      "totalPoint": 29952,
      "profilePicture": "enth/638818232516312348.png",
      "gender": "Male",
      "rank": 1,
      "level": "Grand Master",
      "maximumLevelPoint": 1000,
      "levelCode": "LEVEL5",
      "houseCode": "GREEN",
      "houseName": "Green House",
      "eId": "1hYJXXhSkF5gojB+LP0NgA==",
      "country": null,
      "createdDate": "2025-05-09T14:58:43"
    }
  ]
}
```

### 5. Get Category Rankings
- **Endpoint**: `POST /api/v1/User/GetCategoryRanking`
- **URL**: `https://gogetempowered.com/api/v1/User/GetCategoryRanking`
- **Authentication**: Bearer Token
- **Payload**: 
  ```json
  {"ranks":10,"configuredColumnName":"","houseCode":null,"configuredColumnValue":""}
  ```
- **Response**: Array of ranked users by category
 ```json
{
  "topRanking": [
    {
      "userId": 0,
      "euSerId": "YHSkA+oXyG5awnev610Vsw==",
      "userName": "Narendra Shete",
      "totalPoint": 20,
      "profilePicture": "",
      "gender": "",
      "rank": 1,
      "level": "Knight 2",
      "maximumLevelPoint": 50,
      "levelCode": "LEVEL1",
      "houseCode": "YELLOW",
      "houseName": "Yellow House",
      "eId": "zuyN1moDThcHeUtBaFEhDA==",
      "country": null,
      "createdDate": "2024-07-17T16:48:55"
    }
  ]
}
```

---

## Explore

### 6. Get All Categories
- **Endpoint**: `GET /api/v1/Category/-1/-1/`
- **URL**: `https://gogetempowered.com/api/v1/Category/-1/-1/`
- **Authentication**: Bearer Token
- **Response**: Array of categories
```json
[
    {
        "id": 179,
        "code": "526",
        "name": "Comprehensive Career Programs",
        "imagePath": "enth/thumbnail/course/638575840919183387.png",
        "sequenceNo": 1
    }
]
```

### 7. Get Subcategories
- **Endpoint**: `GET /api/v1/SubCategory/-1/-1/null/{categoryId}/`
- **URL**: `https://gogetempowered.com/api/v1/SubCategory/-1/-1/null/{categoryId}/`
- **Authentication**: Bearer Token
- **Response**: Array of subcategories
```json
[
    {
        "id": 425,
        "categoryId": 178,
        "code": "SITWD",
        "name": "Product training",
        "categoryName": "Software,IT and Web Development ",
        "sequenceNo": 1,
        "thumbnailPath": null
    }
]
```

### 8. Get Category Courses
- **Endpoint**: `GET /api/v1/mycourses/{page}/{pagesize}/{categoryId}/null/null/null/null/true/true/recently/null/All/null/null/null/null`
- **URL**: `https://gogetempowered.com/api/v1/mycourses/{page}/{pagesize}/{categoryId}/null/null/null/null/true/true/recently/null/All/null/null/null/null`
- **Authentication**: Bearer Token
- **Response**: Array of courses in category
 ```json
[
    {
        "courseId": 16447,
        "title": "gamefication_normal",
        "mission": null,
        "description": "<p>learn about LMS</p>",
        "thumbnailPath": "/assets/img/Thumbnail_vectors/img_thumb26.jpg",
        "categoryName": "Software, IT and Web Development",
        "subCategoryName": "Product training",
        "subSubCategoryName": "LMS training",
        "code": "7026",
        "courseFee": 0.0,
        "currency": "",
        "courseType": "elearning",
        "completionPeriodDays": 3,
        "courseCreationdDays": 0,
        "numberofModules": 2,
        "categoryId": 178,
        "subCategoryId": 425,
        "subSubCategoryId": null,
        "courseRating": 0.0,
        "status": null,
        "isFeedback": false,
        "isAssignment": false,
        "isAssessment": false,
        "isPreAssessment": false,
        "isCertificateIssued": true,
        "courseStartDate": null,
        "courseCompleteDate": null,
        "rewardPoint": null,
        "isCourseApplicable": false,
        "courseApprovalStatus": "",
        "competencyCategory": "--",
        "competencyCategoryID": 0,
        "assessmentPercentage": null,
        "scheduleRequestStatus": "",
        "durationInMinutes": 0,
        "assessmentResult": null,
        "isPreRequisiteCourse": false,
        "isExternalProvider": false,
        "externalProvider": null,
        "courseURL": "",
        "isRetraining": false,
        "nodalApprovalStatus": "Not Requested",
        "isSCORM": false,
        "firstAccessDate": null,
        "lastAccessDate": null,
        "timeSpent": null,
        "views": 0,
        "progressinpercentage": 0,
        "score": 0,
        "assignmentType": "",
        "courseDueDate": "NA",
        "alreadyEnrolled": null,
        "certificationStatus": null
    }
]
```

---

## Knowledge Library

### 9. Get News Updates
- **Endpoint**: `GET /api/v1/NewsUpdates`
- **URL**: `https://gogetempowered.com/api/v1/NewsUpdates`
- **Authentication**: Bearer Token

### 10. Get Media Library
- **Endpoint**: `POST /api/v1/MediaLibrary/AlbumsV2`
- **URL**: `https://gogetempowered.com/api/v1/MediaLibrary/AlbumsV2`
- **Authentication**: Bearer Token
- **Payload**: 
  ```json
  {"page":-1,"pageSize":-1,"search":""}
  ```
- **Response**: Array of media albums
  ```json
  {
    "records": [
      {
        "id": 93,
        "albumName": "test video file"
      }
    ]
  }
  ```
  ### 11. Get Quize Corner
- **Endpoint**: `GET api/v1/QuizzesManagement/GetAllQuizzesManagementForEndUser`
- **URL**: `https://gogetempowered.com/api/v1/QuizzesManagement/GetAllQuizzesManagementForEndUser`
- **Authentication**: Bearer Token
- **Response**: 
```json
[
  {
    "id": 1082,
    "date": "0001-01-01T00:00:00",
    "quizTitle": "Test 2022 Quiz ",
    "applicabilityParameter": null,
    "applicabilityParameterValue": null,
    "applicabilityParameterValueId": null,
    "targetResponseCount": 0,
    "status": false
  },
  {
    "id": 1090,
    "date": "0001-01-01T00:00:00",
    "quizTitle": "demo 12345",
    "applicabilityParameter": null,
    "applicabilityParameterValue": null,
    "applicabilityParameterValueId": null,
    "targetResponseCount": 0,
    "status": false
  }
]
```

### 12. Get Survey Corner

- **Endpoint**: `GET /api/v1/SurveyManagement/GetAllSurveyManagementForEndUser`
- **URL**: `https://gogetempowered.com`
- **Authentication**: Bearer Token required

### 13. Get News Updates

- **Endpoint**: `GET /api/v1/NewsUpdates`
- **URL**: `https://gogetempowered.com/api/v1/PollsManagement/GetAllPollsManagementForEndUser`
- **Authentication**: Bearer Token

### 14. Get Polls Corner
- * **Endpoint**: `GET /api/v1/PollsManagement/GetAllPollsManagementForEndUser`
-  **URL**: `https://gogetempowered.com/api/v1/PollsManagement/GetAllPollsManagementForEndUser`
- **Authentication**: Bearer Token

### 15. Get Publications by Folder

- **Endpoint**: `GET /api/v1/Publications/GetAllPublicationsByFolders/{folderId}`
- **URL**: `https://gogetempowered.com/api/v1/Publications/GetAllPublicationsByFolders/null`
- **Authentication**: Bearer Token 
---
### 16. Get Social File

* **Endpoint**: `POST /api/v1/Publications/GetSocialFile`
* **URL**: `https://gogetempowered.com/api/v1/Publications/GetSocialFile`
* **Authentication**: Bearer Token required
* **Request Body** (JSON):

  ```json
  {
    "socialfile": "/enth/Publication/.pdf/638779104850058669.pdf"
  }
  ```
* **Description**:
  Retrieves the specified social PDF file (typically for viewing or downloading).

  
### 17. Get Central Book Library Categories

- **Endpoint**: `GET /api/v1/CentralBookLibrary/GetAllCategory`
- **URL**: `https://gogetempowered.com/api/v1/CentralBookLibrary/GetAllCategory`
- **Authentication**: Bearer Token required

- **Response**: 
```json
[
  {
    "id": 1,
    "category": "Product Management"
  },
  {
    "id": 2,
    "category": "Communication"
  }
]
```
### 18. Get Configurable Parameter Value – SHOW\_POLICYLABEL

- **Endpoint**: `GET /api/v1/ConfigurableParameters/GetValue/SHOW_POLICYLABEL`
- **URL**: `https://gogetempowered.com/api/v1/ConfigurableParameters/GetValue/SHOW_POLICYLABEL`
- **Authentication**: Bearer Token required

- **Response**: 

```json
{
  "value": "Yes"
}
```


### 19. Get Policy Document

- **Endpoint**: `GET /api/v1/PolicyDocument`
- **URL**: `https://gogetempowered.com/api/v1/PolicyDocument`
- **Authentication**: Bearer Token required

```json
[
  {
    "customerCode": null,
    "applicabilityParameter": null,
    "applicabilityParameterValue": null,
    "applicabilityParameterValueId": null,
    "id": 4,
    "policyId": "enth4",
    "policyDescription": "Quality",
    "commanToAllUser": true,
    "modifiedDate": "11/10/2022 7:05:33 AM",
    "reviewFrequency": "Monthly",
    "ruleId": "Quality4",
    "conditionRegardToOtherRules": "",
    "contentPath": "/enth/.pdf/638036805198254935..pdf",
    "policyLabel": "policy d"
  }
]
```
### 20. Get My Courses 
* **Endpoint**:  
  `GET /api/v1/mycourses/{page}/{pageSize}/null/null/null/null/null/null/true/a-z/null/All/null/null/null/null`

* **URL**:  
  `https://gogetempowered.com/api/v1/mycourses/1/10/null/null/null/null/null/null/true/a-z/null/All/null/null/null/null`

* **Authentication**: Bearer Token

* **Response**:
```json
[
  {
    "courseId": 13014,
    "title": "2004",
    "description": "<p>anfjs fdmngjrf dngtltrif sndjf wjsdinc vbfhudsd ndflkj</p>",
    "thumbnailPath": "../../../assets/img/Thumbnail_vectors/img_thumb150.jpg",
    "courseType": "elearning",
    "categoryName": "--",
    "courseFee": 0.0,
    "numberofModules": 1,
    "courseRating": 0.0,
    "isCertificateIssued": true,
    "progressinpercentage": 0,
    "score": 0,
    "courseDueDate": "NA",
    "isSCORM": true,
    "nodalApprovalStatus": "Not Requested"
  }
]
```
## Catalog

### 8.1 Get My Courses
* **Endpoint**:  
  `GET /api/v1/mycourses/{page}/{pageSize}/null/null/null/null/null/null/true/a-z/null/All/null/null/null/null`

* **URL**:  
  `https://gogetempowered.com/api/v1/mycourses/1/10/null/null/null/null/null/null/true/a-z/null/All/null/null/null/null`

* **Authentication**: Bearer Token
* **Response**:
```json
[
  {
    "courseId": 13014,
    "title": "2004",
    "mission": null,
    "description": "<p>anfjs fdmngjrf dngtltrif sndjf wjsdinc vbfhudsd ndflkj</p>",
    "thumbnailPath": "../../../assets/img/Thumbnail_vectors/img_thumb150.jpg",
    "categoryName": "--",
    "subCategoryName": "",
    "subSubCategoryName": "",
    "code": "5004",
    "courseFee": 0.0,
    "currency": "",
    "courseType": "elearning",
    "completionPeriodDays": 0,
    "courseCreationdDays": 0,
    "numberofModules": 1,
    "categoryId": null,
    "subCategoryId": 0,
    "subSubCategoryId": null,
    "courseRating": 0.0,
    "status": null,
    "isFeedback": false,
    "isAssignment": false,
    "isAssessment": false,
    "isPreAssessment": false,
    "isCertificateIssued": true,
    "isSCORM": true,
    "progressinpercentage": 0,
    "score": 0,
    "courseDueDate": "NA",
    "nodalApprovalStatus": "Not Requested"
  }
]
```

### 8.2 Get Course Count
* **Endpoint**:  
  `GET /api/v1/mycourses/count/null/null/null/null/null/null/true/a-z/null/All/null/null/null/null`

* **URL**:  
  `https://gogetempowered.com/api/v1/mycourses/count/null/null/null/null/null/null/true/a-z/null/All/null/null/null/null`

* **Authentication**: Bearer Token

* **Response**:  
  `1284` (Total course count as integer)

### 8.3 Get Selected Languages
* **Endpoint**:  
  `GET /api/v1/Customer/GetSelectedLanguages`

* **URL**:  
  `https://gogetempowered.com/api/v1/Customer/GetSelectedLanguages`

* **Authentication**: Bearer Token

* **Response**:
```json
[
  {
    "code": "en",
    "isDeleted": false,
    "name": "English"
  },
  {
    "code": "ar",
    "isDeleted": false,
    "name": "Arabic"
  }
]
```

### 8.4 Get Course Enrollment Config
* **Endpoint**:  
  `GET /api/v1/ConfigurableParameters/GetValue/COURSE_ENROLL`

* **URL**:  
  `https://gogetempowered.com/api/v1/ConfigurableParameters/GetValue/COURSE_ENROLL`

* **Authentication**: Bearer Token

* **Response**:
```json
{
  "value": "TrainingRequest"
}
```

### 8.5 Get All Categories 
* **Endpoint**:  
  `GET /api/v1/Category`

* **URL**:  
  `https://gogetempowered.com/api/v1/Category`

* **Authentication**: Bearer Token

* **Response**:
```json
[
  {
    "id": 179,
    "code": "526",
    "name": "Comprehensive Career Programs",
    "imagePath": "enth/thumbnail/course/638575840919183387.png",
    "sequenceNo": 1
  },
  {
    "id": 178,
    "code": "079",
    "name": "Software,IT and Web Development",
    "imagePath": "enth/thumbnail/course/638575389614925644.png",
    "sequenceNo": 2
  }
]
```
## Subset of Subcategories

### 1.Get All Categories

**Endpoint:**

```
GET /api/v1/Category
```

**Example Response:**

```json
[
  {
    "id": 178,
    "name": "Software,IT and Web Development"
  }
]
```

---

### 2.Get Subcategories by Category

**Endpoint:**

```
GET /api/v1/SubCategory/GetSubCategoryByCategory/{categoryId}
```

**Example:**

```
GET /api/v1/SubCategory/GetSubCategoryByCategory/178
```

**Response:**

```json
[
  {
    "id": 425,
    "name": "Product training"
  }
]
```

---

### 3.Create a SubSubCategory (Subset)

**Endpoint:**

```
POST /api/v1/c/SubSubCategory
```

**Payload Example:**

```json
{
  "id": null,
  "categoryId": 178,
  "subCategoryId": 425,
  "code": "287",
  "name": "SQL SERVER",
  "categoryName": null,
  "subCategoryName": null
}
```
### 4.List All SubSubCategories

**Endpoint:**

```
GET /api/v1/c/SubSubCategory/1/10/null/null/null/
```

**Response Example:**

```json
[
  {
    "id": 447,
    "categoryId": 178,
    "subCategoryId": 425,
    "code": "PT",
    "name": "LMS training"
  }
]
```

---

### 5.Get Total SubSubCategory Count

**Endpoint:**

```
GET /api/v1/c/SubSubCategory/count
```


## Competency 

### 9.1 Get Competency Hub Data 
* **Endpoint**: `POST /api/v1/Report/Competency/GetCompetencyHubData`
* **URL**: `https://gogetempowered.com/api/v1/Report/Competency/GetCompetencyHubData`
* **Authentication**: Bearer Token
* **Payload**:
```json
{"Page":1,"PageSize":10}
```
* **Response(Trimed responce)**:
```json
{
  "success": true,
  "data": {
    "records": [
      {
        "categoryName": "negotiation skills",
        "competencyName": "bargaining",
        "competencyID": "288",
        "requiredLevel": "Level 1"
      },
      {
        "categoryName": "Recruiter",
        "competencyName": "Channel",
        "competencyID": "314",
        "requiredLevel": "Level 1"
      }
    ]
  }
}
```

### 9.2 Get Competency Spider Chart 
* **Endpoint**: `GET /api/v1/CompetencyCategory/GetCompetencySpiderchart`
* **URL**: `https://gogetempowered.com/api/v1/CompetencyCategory/GetCompetencySpiderchart`
* **Authentication**: Bearer Token
* **Response(Trimed responce)**:
```json
{
  "counts": [66.67, 50.0, 100.0],
  "competencyName": [
    "Collaboration",
    "Excellence Orientation",
    "Customer Focus"
  ]
}
```

## Calendar

### 10.1 Get Date Format 
* **Endpoint**: `GET /api/v1/ConfigurableParameters/GetValue/APPLICATION_DATE_FORMAT`
* **Response**: 
```json
{"value":"dd MMM yyyy"}
```

### 10.2 Get ILT Calendar Data 
* **Endpoint**: `POST /api/v1/calendar/ILTCalenderData`
* **Payload**:
```json
{"fromDate":"2025-05-01T00:00:00.000Z","toDate":"2025-06-29T18:30:00.000Z"}
```

### 10.3 Check Batch Nomination Status
* **Endpoint**: `GET /api/v1/c/ILTBatch/IsBatchwiseNominationEnabled`
* **Response**: `"No"`

### 10.4 Get Calendar Help Info
* **Endpoint**: `GET /api/v1/QuickHelpInfo/GetHelpByType/l_cal`

### 10.5 Get Academy List
* **Endpoint**: `GET /api/v1/ILTSchedule/GetAcademyTypeAhead/Internal`
* **Response**:
```json
[
  {"id":1,"title":"MIT"},
  {"id":2,"title":"Enthralltech"}
]
```

### 10.6 Get Organization Calendar
* **Endpoint**: `POST /api/v1/calendar/OrganizationCalenderData`
* **Payload**:
```json
{"fromDate":"2025-05-01T00:00:00.000Z","toDate":"2025-06-29T18:30:00.000Z"}
```
* **Response**:
```json
[
  {
    "courseId": 9734,
    "moduleName": "3742_VILT Type Course",
    "moduleType": "vilt"
  }
]
```

### 10.7 Export ILT Calendar
* **Endpoint**: `POST /api/v1/calendar/ILTCalenderDataExport`
* **Payload**:
```json
{"fromDate":"2025-05-01T00:00:00.000Z","toDate":"2025-06-29T18:30:00.000Z"}
```

### 10.8 Export Trainer Calendar
* **Endpoint**: `POST /api/v1/calendar/ILTCalenderDataForTrainerExport`
* **Payload**: Same as 10.7

### 10.9 Get Schedule Data
* **Endpoint**: `POST /api/v1/ILTSchedule/GetScheduleData`
* **Payload**:
```json
{"Page":1,"PageSize":10,"showAllData":"false"}
```
* **Response**:
```json
[
  {
    "id": 7020,
    "startDate": "2025-05-12T00:00:00",
    "startTime": "15:50:00"
  }
]
```

### 10.10 Get Schedule Count
* **Endpoint**: `GET /api/v1/ILTSchedule/count/null/null/false`
* **Response**: `753`

### 10.11 Check Past Schedule Cancellation
* **Endpoint**: `GET /api/v1/ConfigurableParameters/GetValue/Enable_PastScheduleCancel`
* **Response**: 
```json
{"value":"Yes"}
```

### 10.12 Get Localization Strings
* **Endpoint**: `GET /assets/i18n/en.json`
* **Response**:
```json
{
  "SUBMIT_ASSIGNMENT": "Please submit assignment...",
  "CUSTOMER": {
    "HEADER": "Customer Master"
  }
}
```

### 10.13 Get Nomination Data
* **Endpoint**: `POST /api/v1/TrainingNomination/GetNominationData`
* **Payload**:
```json
{"page":1,"pageSize":10,"showAllData":"false"}
```
* **Response**:
```json
[
  {
    "id": 7019,
    "startDate": "2025-05-05T00:00:00"
  }
]
```

### 10.14 Get Nomination Count
* **Endpoint**: `GET /api/v1/TrainingNomination/count/null/null/false`
* **Response**: `622`

### 10.15 Get Training Attendance
* **Endpoint**: `GET /api/v1/ILTTrainingAttendance/1/10/null/null/false`
* **Response**:
```json
[
  {
    "scheduleCode": "SC12745",
    "startDate": "2025-05-12T00:00:00"
  }
]
```

## Profile

### 11.1 Get Encrypted User ID {#111-get-encrypted-user-id}
* **Endpoint**: `POST /api/v1/User/GetEncryptedUserId`
* **Payload**: `{}`
* **Response**:
```json
{"encryptedUserId":"fk2zuGnuQ/lJ2By+PLvNTg=="}
```

### 11.2 Get Profile Permissions

* **Endpoint**: `GET /api/v1/user/GetProfilePermission`
* **Response**:
```json
[
  {
    "name": "Change Password",
    "code": "ch_pass",
    "isAccess": true
  }
]
```

### 11.3 Get User Configurable Parameters
* **Endpoint**: `POST /api/v1/user/UserConfigurableParameter`
* **Payload**:
```json
["HRBP_Rename","Mentor_Rename"]
```
* **Response**:
```json
[
  {
    "code": "HRBP_Rename",
    "value": "HRBP"
  }
]
```

### 11.4 Check Federation ID Status 
* **Endpoint**: `GET /api/v1/ConfigurableParameters/GetValue/Enable_FederationID`
* **Response**: 
```json
{"value":"No"}
```

### 11.5 Get User Profile
* **Endpoint**: `GET /api/v1/user/GetUserProfile`
* **Response**:
```json
{
  "userName": "LMS Admin",
  "timeZone": "(UTC+05:30) Chennai...",
  "profilePicture": ""
}
```

### 11.6 Get User Settings
* **Endpoint**: `GET /api/v1/user/UserSetting/1/25`
* **Response**:
```json
[
  {
    "configuredColumnName": "Business",
    "fieldType": "TYPEAHEAD"
  }
]
```

### 11.7 Get Profile Picture 
* **Endpoint**: `POST /api/v1/User/GetProfilePicture`
* **Payload**: `{"id":""}`

### 11.8 Get User Details by ID 
* **Endpoint**: `POST /api/v1/User/GetUserDetailsById`
* **Payload**:
```json
{"id":"fk2zuGnuQ/lJ2By+PLvNTg=="}
```
* **Response**:
```json
{
  "userName": "LMS Admin",
  "profilePicture": "enth/638818232516312348.png"
}
```

### 11.9 Get Competency Status Report
* **Endpoint**: `POST /api/v1/Report/Competency/CompetencyStatusReport/Self`
* **Payload**:
```json
{"Page":1,"PageSize":10}
```
* **Response**:
```json
{
  "competencyCharts": [
    {
      "competencyName": "Collaboration",
      "status": "Pending"
    }
  ]
}
```

### 11.10 Get Key Area Settings Count 
* **Endpoint**: `GET /api/v1/KeyAreaSetting/GetMyKeyAreaSettingCount/`
* **Response**: `0`

### 11.11 Get Key Area Settings
* **Endpoint**: `GET /api/v1/KeyAreaSetting/GetMyKeyAreaSetting/1/10/`
* **Response**: `[]`

### 11.12 Check External Certificate Status 
* **Endpoint**: `GET /api/v1/ConfigurableParameters/GetValue/ExternalCertificate`
* **Response**: 
```json
{"value":"Yes"}
```

### 11.13 Get User Certificates
* **Endpoint**: `GET /api/v1/CourseCertificateAssociation/GetUserCertificatesByUserId/1/10/null/null`
* **Response**:
```json
[
  {
    "id": 4,
    "category": null
  }
]
```

### 11.14 Get User Certificates Count
* **Endpoint**: `GET /api/v1/CourseCertificateAssociation/GetUserCertificatesByUserIdCount/null/null`
* **Response**: `4`

### 11.15 Check VIMEO Status
* **Endpoint**: `GET /api/v1/ConfigurableParameters/GetValue/VIMEO`
* **Response**: 
```json
{"value":"No"}
```

### 11.16 Upload Profile Picture
* **Endpoint**: `POST /api/v1/user/ProfilePictureUpload`
* **Authentication**: Bearer Token
* **Content-Type**: `application/json`
* **Payload**:
```json
{
  "base64String": "data:image/png;base64,iVBORw0KGgo...",
  "customerName": null,
  "url": null
}
```

### 11.17 Get Profile Picture Size Limit
* **Endpoint**: `GET /api/v1/MasterPageSetting/GetFileFormatSize/USER_PROFILE`
* **Response**:
```json
{
  "id": 2,
  "name": "USER_PROFILE",
  "size": 3072
}
```



## Course Management 


### 12.1 Get LCMS Media 
* **Endpoint**: `POST /api/v1/LCMS/GetLCMSMedia`
* **Payload**:
```json
{
  "page": 1,
  "pageSize": 18,
  "search": "scorm",
  "showAllData": "false"
}
```
* **Response**:
```json
{
  "data": [
    {
      "id": 16004,
      "name": "Day 1_About_Max_12May_NOQus_2004",
      "path": "/assets/courses/638826713822767440Day1_About_Max_12May_NOQus_2004/index_lms.html",
      "contentType": "SCORM1.2",
      "isMobileCompatible": true
    }
  ]
}
```

### 12.2 Get File Format Size
* **Endpoint**: `GET /api/v1/MasterPageSetting/GetFileFormatSize/ADDITIONAL_RESOURCE`
* **Response**:
```json
{
  "id": 28,
  "name": "ADDITIONAL_RESOURCE",
  "size": 51200
}
```

### 12.3 Get Media Count
* **Endpoint**: `GET /api/v1/LCMS/GetMediaCount/true`
* **Response**: Returns integer count of media items


### 12.4 Upload SCORM Content
* **Endpoint**: `POST /api/v1/LCMS`
* **Authentication**: Bearer Token
* **Content-Type**: `multipart/form-data`
* **Required Parameters**:

| Field | Type | Description | Example |
|-------|------|-------------|---------|
| `name` | string | Course name | "History of Agra" |
| `description` | string | Course description | "Journey of Agra to become a National Heritage site" |
| `contentType` | string | MIME type of content | "application/x-zip-compressed" |
| `version` | string | Content version | "1.0" |
| `metaData` | string | Additional metadata | "Indian Historical place" |
| `language` | string | Language code | "en" |
| `scormType` | string | SCORM version | "SCORM1.2" |
| `duration` | integer | Duration in minutes | 60 |
| `isMobileCompatible` | boolean | Mobile compatibility | true |
| `fileForUpload` | binary | ZIP file containing SCORM package | test.zip |

* **Optional Parameters**:
  - `youtubeVideoId`: (string) YouTube video ID if applicable
  - `isBuiltInAssessment`: (boolean) Default false
  - `isSecuredContent`: (boolean) Default false

* **Success Response**: 1

### 12.5 Upload PDF Content
* **Endpoint**: `POST /api/v1/LCMS`
* **Authentication**: Bearer Token required
* **Content-Type**: `multipart/form-data`
* **Request Parameters**:

| Field | Type | Required | Description | Example |
|-------|------|----------|-------------|---------|
| `name` | string | Yes | Content title | "sahich" |
| `description` | string | Yes | Content description | "How sahich became top hotel industry" |
| `contentType` | string | Yes | Must be "application/pdf" | "application/pdf" |
| `version` | string | Yes | Content version | "1.0" |
| `originalFileName` | string | Yes | Original PDF filename | "Document.pdf" |
| `language` | string | Yes | 2-letter language code | "en" |
| `duration` | integer | Yes | Duration in minutes | 60 |
| `fileForUpload` | binary | Yes | PDF file content | - |


### 12.6 Content Size Limits
* **Endpoint**: `GET /api/v1/MasterPageSetting/GetFileFormatSize/{type}`
* **Supported Types**:
  | Content Type       | Max Size | Example Response |
  |--------------------|----------|------------------|
  | `NON_SCORM`        | 1.5GB    | `{"id":8,"size":1572864}` |
  | `H5P`              | 500MB    | `{"id":9,"size":512000}` |
  | `VIDEO`            | 400MB    | `{"id":11,"size":409600}` |
  | `PODCAST`          | 3MB      | `{"id":12,"size":3072}` |
  | `ADDITIONAL_RESOURCE` | 50MB | `{"id":28,"size":51200}` |

### 12.7 H5P Content
* **Endpoint**: `POST /api/v1/LCMS/GetLCMSMedia`
* **Payload**:
```json
{"page":1,"pageSize":18,"search":"h5p"}
```
* **Response**:
```json
{
  "data": [{
    "id": 13577,
    "name": "H5P Module",
    "path": "/assets/h5pcourses/...",
    "contentType": "h5p"
  }]
}
```

### 12.8 Video Content
* **Endpoint**: `POST /api/v1/LCMS/GetLCMSMedia`
* **Vimeo Status Check**:
  ```bash
  GET /api/v1/ConfigurableParameters/GetValue/VIMEO
  ```
  ```json
  {"value":"No"}
  ```

### 12.9 Survey Content {#129-survey-content}
* **Get Surveys**:
  ```bash
  GET /api/v1/LCMS/GetMedia/1/10/survey
  ```
* **Total Records**:
  ```bash
  GET /api/v1/SurveyManagement/SurveyQuestion/GetTotalRecords
  ```
  ```json
  173
  ```

### 12.10 Audio/Podcast
* **Endpoint**: `POST /api/v1/LCMS/GetLCMSMedia`
* **Payload**:
```json
{"search":"audio"}
```
* **Response**:
```json
{
  "data": [{
    "path": "https://.../audio.wav",
    "contentType": "audio"
  }]
}
```

### 12.11 YouTube Integration 
* **Endpoint**: `POST /api/v1/LCMS/GetLCMSMedia`
* **Response**:
```json
{
  "data": [{
    "youtubeVideoId": "YIhtkEjFOG8",
    "contentType": "youtube"
  }]
}
```

### 12.12 External Links
* **Endpoint**: `POST /api/v1/LCMS/GetLCMSMedia`
* **Response**:
```json
{
  "data": [{
    "path": "https://example.com/faq",
    "contentType": "externallink"
  }]
}
```

### 12.13 Assignments
* **Endpoint**: `POST /api/v1/LCMS/GetLCMSMedia`
* **Payload**:
```json
{"search":"assignment"}
```
* **Response**:
```json
{
  "data": [{
    "name": "Test Assignment",
    "contentType": "assignment"
  }]
}
```

## Edit Course

### 1. Get Course Details for Editing

**Endpoint:**

```
GET /api/v1/courses/GetCourseDetailsForUpdate/{courseId}
```

**Example:**

```
GET /api/v1/courses/GetCourseDetailsForUpdate/20213
```

**Response (trimmed):**

```json
{
  "id": 20213,
  "code": "8130",
  "title": "Day1_About_Max_noGUI",
  "courseType": "elearning",
  "courseAdminID": 2549,
  "isCertificateIssued": false,
  "completionPeriodDays": 0
}
```

---

### 2. Get Course Competency Skills

**Endpoint:**

```
GET /api/v1/courses/GetCompetencySkillByCourseId/{courseId}
```

---

### 3. Get Course SubSubCategory

**Endpoint:**

```
GET /api/v1/courses/GetSubSubCategoryByCourseId/{courseId}
```

---

###  4. Check Refresher Config

**Endpoint:**

```
GET /api/v1/ConfigurableParameters/GetValue/REFRESHER
```

---

### 5. Get Course Categories

**Endpoint:**

```
GET /api/v1/Category
```

---

### 6. Get Linked Course Modules

**Endpoint:**

```
GET /api/v1/courses/GetCoursesModules/{courseId}
```

**Response (trimmed):**

```json
[
  {
    "id": 24314,
    "moduleId": 18503,
    "isAssessment": false
  }
]
```

---

### 7. Get Course Assessments & Feedback Names

**Endpoint:**

```
GET /api/v1/Courses/GetCoursesAssessmentFeedbackName/null/null/null/null/null/null
```

**Response (trimmed):**

```json
{
  "assessmentName": null,
  "feedbackName": null
}
```

---

### 8. Get Section by Course Code

**Endpoint:**

```
GET /api/v1/section/{courseCode}
```

---

### 9. Check EdCast Enabled

**Endpoint:**

```
GET /api/v1/ConfigurableParameters/GetValue/Enable_Edcast
```

**Response:**

```json
{ "value": "No" }
```

---

### 10. Get Vendor Details

**Endpoint:**

```
POST /api/v1/courses/GetCourseVendorDetails
```

**Payload:**

```json
{ "Vendor_Type": "Internal" }
```

**Response (trimmed):**

```json
[
  {
    "code": "V001",
    "name": "EnthrallTech",
    "id": 1
  }
]
```

---

### 11. Get Modules (by Search)

**Endpoint:**

```
POST /api/v1/module/GetModuleData
```

**Payload (example):**

```json
{
  "page": 1,
  "pageSize": 5,
  "search": "Classroom",
  "columnName": "coursetype",
  "showAllData": true
}
```

---

### 12. Save/Update Course

**Endpoint:**

```
POST /api/v1/courses/{courseId}
```

**Example:**

```
POST /api/v1/courses/20214
```

**Payload (trimmed):**

```json
{
  "id": 20214,
  "title": "demo courses classroom",
  "courseType": "Classroom",
  "courseAdminIDs": ["2549"],
  "isCertificateIssued": false,
  "moduleAssociation": [
    {
      "moduleId": 18503,
      "isAssessment": false
    }
  ],
  "vendorId": 1,
  "vendorName": "EnthrallTech"
}
```

**Response:**

```json
1
```

---


## Module Management

### 13.1 Get Module Data
* **Endpoint**: `POST /api/v1/module/GetModuleData`
* **Authentication**: Bearer Token
* **Payload**:
```json
{
  "page": 1,
  "pageSize": 10,
  "showAllData": "false"
}
```
* **Response**:
```json
{
  "data": [
    {
      "id": 18498,
      "name": "sahich",
      "moduleType": "Document",
      "description": "sahich",
      "isActive": true,
      "createdBy": 2549,
      "userName": "LMS Admin"
    }
  ]
}
```

### 13.2 Get Media Count
* **Endpoint**: `GET /api/v1/LCMS/GetMediaCount/true`
* **Authentication**: Bearer Token
* **Response**:
```json
{
  "data": [
    {
      "id": 16004,
      "name": "Day 1_About_Max_12May_NOQus_2004",
      "contentType": "SCORM1.2",
      "isMobileCompatible": true,
      "duration": 60.0
    }
  ]
}
```

### 13.3 Search LCMS Media
* **Endpoint**: `POST /api/v1/LCMS/GetLCMSMedia`
* **Authentication**: Bearer Token
* **Payload**:
```json
{
  "page": 1,
  "pageSize": 12,
  "search": "scorm",
  "showAllData": "false"
}
```
* **Response**:
```json
{
  "data": [
    {
      "id": 16004,
      "name": "Day 1_About_Max_12May_NOQus_2004",
      "path": "/assets/courses/.../index_lms.html",
      "contentType": "SCORM1.2",
      "duration": 60.0,
      "language": "en"
    }
  ]
}
```

## 14. Assessment Attempt Management


### 1. Get All Assessment Attempts

**Endpoint:**

```
GET /api/v1/AssessmentAttemptManagement/{page}/{pageSize}
```

**Example:**

```
GET /api/v1/AssessmentAttemptManagement/1/10
```

**Response (trimmed):**

```json
[
  {
    "id": 1042,
    "courseId": 18782,
    "courseName": "Assessment iLearn",
    "userName": "Danish Hussain",
    "additionalAttempts": 2,
    "isExhausted": false
  }
]
```

---

### 2. Get Assessment Attempt Count

**Endpoint:**

```
GET /api/v1/AssessmentAttemptManagement/Count
```

**Response:**

```json
43
```

---

### 3. Get Modules for Assessment Course

**Endpoint:**

```
GET /api/v1/Module/GetModulesForAssessmentCourses/{courseId}
```

**Example:**

```
GET /api/v1/Module/GetModulesForAssessmentCourses/20177
```

**Response (trimmed):**

```json
[
  { "id": 18434, "title": "EFS PPT Testing" },
  { "id": 18436, "title": "EFS PPT Testing 2" }
]
```

---

### 4. Search Active or Inactive User

**Endpoint:**

```
POST /api/v1/user/searchActiveInActiveUser
```

**Payload:**

```json
{
  "userId": "aX0NGaBB7+oaZe8Bv7m2yQ==",
  "userType": "Z5pxA9AnsHK8ffqkKF9c9Q=="
}
```

**Response (trimmed):**

```json
[
  {
    "name": "LMS Admin",
    "userType": "Internal",
    "isDeleted": false
  }
]
```

---

### 5. Add Assessment Attempt

**Endpoint:**

```
POST /api/v1/AssessmentAttemptManagement
```

**Payload:**

```json
{
  "id": 0,
  "courseId": 20177,
  "courseName": "test assessment 0101",
  "userId": 2549,
  "userName": "LMS Admin",
  "additionalAttempts": 10,
  "ModuleId": 18434
}
```

---

### 6. Upload Attempt File

**Endpoint:**

```
POST /api/v1/AssessmentAttemptManagement/PostFileUpload
```

**Payload:** File upload (example: LearnerCalendarData.xlsx)

**Response:**

```json
"/enth/4.5/xlsx/638827453663167559.xlsx"
```

---

### 7. Download Template File

**Endpoint:**

```
GET /api/v1/AssessmentAttemptManagement/DownloadFile
```

---

### 8. Save Uploaded File Data

**Endpoint:**

```
POST /api/v1/AssessmentAttemptManagement/SaveFileData
```

**Payload:**

```json
{
  "Path": "/enth/4.5/xlsx/638827453959710171.xlsx"
}
```

**Response (trimmed):**

```json
[
  {
    "courseCode": "3742",
    "courseName": "VILT Type Course",
    "errMessage": "UserId not found. Please enter valid data."
  }
]
```

---



## 15 MicroLearning


### 1. Get MicroLearning List (Paginated)

**Endpoint:**

```
GET /api/v1/AuthoringMaster/{page}/{pageSize}
```

**Example:**

```
GET /api/v1/AuthoringMaster/1/10
```

**Response (trimmed):**

```json
[
  {
    "id": 1286,
    "name": "HONASA",
    "skills": "HONASA",
    "description": "HONASA",
    "duration": 25.0,
    "moduleType": "PPTUpload"
  }
]
```

---

### 2. Get MicroLearning Count

**Endpoint:**

```
GET /api/v1/AuthoringMaster/count
```

**Response:**

```json
231
```

---

### 3. Create MicroLearning Module

**Endpoint:**

```
POST /api/v1/AuthoringMaster
```

**Payload:**

```json
{
  "name": "TESTING",
  "skills": "TESTING API",
  "duration": 60,
  "description": "TESTING PURPOSE",
  "lcmsId": 0,
  "isDeleted": false,
  "moduleType": "Microlearning",
  "metaData": "TESTING PURPOSE"
}
```

**Response:**

```json
1287
```

---

### 4. Get MicroLearning Details by ID

**Endpoint:**

```
GET /api/v1/AuthoringMaster/GetDetailsByAuthoringId/{authoringId}/{page}/{pageSize}/{type}
```

**Example:**

```
GET /api/v1/AuthoringMaster/GetDetailsByAuthoringId/1287/1/10/0
```

**Response:**

```json
[]
```

---

### 5. Get Page Number for MicroLearning

**Endpoint:**

```
GET /api/v1/AuthoringMaster/GetPageNumber/{authoringId}
```

**Example:**

```
GET /api/v1/AuthoringMaster/GetPageNumber/1287
```

**Response:**

```json
0
```

---


## 16 Assessment Report APIs

### 1. Get Configurable Report Parameters

**Endpoint:**

```
GET /api/v1/ConfigurableParameters/GetByParameterType/REPORT/CLIENT
```

**Response (trimmed):**

```json
[
  {
    "code": "SHOW_CONFCOLUMNS_INREPORT",
    "value": "Yes",
    "parameterType": "REPORT"
  },
  {
    "code": "SSR",
    "value": "Yes",
    "parameterType": "REPORT"
  }
]
```

---

### 2. Get Course Data

**Endpoint:**

```
POST /api/v1/courses/GetCourseData
```

**Payload (example):**

```json
{
  "page": 1,
  "pageSize": 300,
  "categoryId": null,
  "IsActive": true,
  "search": "",
  "filter": "",
  "showAllData": "false"
}
```

**Response (trimmed):**

```json
{
  "data": [
    {
      "id": 30465,
      "title": "schedule ilt test",
      "courseType": "Classroom",
      "isActive": true,
      "userName": "Lms Admin",
      "totalModules": 1
    }
  ]
}
```

---

### 3. Get Assessment Result Sheet

**Endpoint:**

```
POST /api/v1/Report/GetAssessmentResultSheet/
```

**Payload:**

```json
{
  "courseId": 20989,
  "startIndex": 1,
  "pageSize": 10
}
```


---

### 4. Get Assessment Result Count

**Endpoint:**

```
POST /api/v1/Report/GetAssessmentResultSheetCount/
```

**Payload:**

```json
{
  "courseId": 20989,
  "startIndex": 1,
  "pageSize": 10
}
```

**Response:**

```json
0
```

---

### 5. Get Assessment Result Graph Data

**Endpoint:**

```
POST /api/v1/Report/GetAssessmentResultSheetGraph
```

**Payload:**

```json
{
  "courseId": 20989,
  "startIndex": 1,
  "pageSize": 10
}
```

**Response:**

```json
{
  "counts": [],
  "results": []
}
```

---

### 6. Export Assessment Result Sheet

**Endpoint:**

```
POST /api/v1/Report/ExportGetAssessmentResultSheet/
```

**Payload:**

```json
{
  "courseId": 20989,
  "startIndex": 1,
  "pageSize": 10,
  "ExportAs": "xlsx"
}
```

---



## 17 Additional Assessment Report APIs


### 1. Get Failed Assessment Result Sheet

**Endpoint:**

```
POST /api/v1/Report/GetFailedAssessmentResultSheet
```

**Payload:**

```json
{
  "courseId": 16152,
  "startIndex": 1,
  "pageSize": 10,
  "status": "Failed"
}
```

**Response:**

```json
{
  "totalRecordCount": 0,
  "data": []
}
```

---

### 2. Get User Assessment Sheet

**Endpoint:**

```
POST /api/v1/Report/GetUserAssessmentSheet
```

**Payload:**

```json
{
  "courseId": 16152,
  "userId": 8795,
  "startIndex": 1,
  "pageSize": 10
}
```

---

### 3. Get User Assessment Sheet Count

**Endpoint:**

```
POST /api/v1/Report/GetUserAssessmentSheetCount/
```

**Payload:**

```json
{
  "courseId": 16152,
  "userId": 8795,
  "startIndex": 1,
  "pageSize": 10
}
```

---

### 4. Get Assessment Response Analysis

**Endpoint:**

```
POST /api/v1/Report/GetAssessmentResponseAnalysis
```

**Payload:**

```json
{
  "courseId": 16152,
  "startIndex": 1,
  "pageSize": 10
}
```

---

## 18 Assessment Response Analysis Report


### 1. Get Assessment Response Analysis

**Endpoint:**

```
POST /api/v1/Report/GetAssessmentResponseAnalysis
```

**Payload:**

```json
{
  "courseId": 16152,
  "startIndex": 1,
  "pageSize": 10,
  "sortOrder": null,
  "count": 0,
  "search": null,
  "moduleId": null,
  "status": null,
  "ExportAs": null
}
```

**Response:**

```json
{
  "list": [],
  "count": 0
}
```


## 19 Assessment Reports

This section provides endpoints for analytical insights like top/bottom performers, course completion, unit-wise stats, and assessment deployment vs completion.

### 1. Get Top 5 Performers Export

**Endpoint:**

```
POST /api/v1/AnalyticalDashboard/GetAssessmentTop5AnalyaticalDashboardExport
```

**Payload:**

```json
{
  "courseIds": [54],
  "graphType": null
}
```

---

### 2. Get Top Performer Graph

**Endpoint:**

```
POST /api/v1/AnalyticalDashboard/GetAssessmentTopPerformerGraph
```

**Payload:**

```json
{
  "courseIds": [54],
  "graphType": null
}
```

---

### 3. Get Bottom 5 Performers Export

**Endpoint:**

```
POST /api/v1/AnalyticalDashboard/GetAssessmentBottom5AnalyaticalDashboardExport
```

**Payload:**

```json
{
  "courseIds": [54],
  "graphType": null
}
```

---

### 4. Get Unit-wise Assessment Report Export

**Endpoint:**

```
POST /api/v1/AnalyticalDashboard/GetAssessmentAnalyaticalDashboardExport
```

**Payload:**

```json
{
  "courseIds": [54],
  "graphType": "Unit"
}
```

---

### 5. Get Unit-wise Assessment Graph

**Endpoint:**

```
POST /api/v1/AnalyticalDashboard/GetAssessmentAnalyticalDashboardGraph
```

**Payload:**

```json
{
  "courseIds": [54],
  "graphType": "Unit"
}
```

---

### 6. Get Course Completion Rate Export

**Endpoint:**

```
POST /api/v1/AnalyticalDashboard/GetCompletionRateExport
```

**Payload:**

```json
{
  "startDate": "2023-02-01T00:00:00",
  "endDate": "2025-02-06T00:00:00"
}
```

---

### 7. Get Course Completion Rate Data

**Endpoint:**

```
POST /api/v1/AnalyticalDashboard/GetCompletionRate
```

**Payload:**

```json
{
  "startDate": "2023-02-01T00:00:00",
  "endDate": "2025-02-06T00:00:00"
}
```

**Response (example):**

```json
[
  {
    "completionRate": 100.0,
    "courseId": "2",
    "courseName": "Practising Business Etiquettes"
  }
]
```

---

### 8. Get Categories (for Filters)

**Endpoint:**

```
GET /api/v1/Category
```

---

### 9. Get Category-wise Report Export

**Endpoint:**

```
POST /api/v1/AnalyticalDashboard/GetCategoryExport
```

**Payload:**

```json
{
  "category1": null,
  "category2": null,
  "category3": null,
  "category4": null,
  "category5": null
}
```

---

### 10. Get Category-wise Report Graph

**Endpoint:**

```
POST /api/v1/AnalyticalDashboard/GetCategoryWiseGraph
```

**Payload:**

```json
{
  "category1": "8"
}
```

---

### 11. Get Deployed vs Completed Assessment Report Export

**Endpoint:**

```
POST /api/v1/AnalyticalDashboard/Export
```

**Payload:**

```json
{
  "startDate": "01 Feb 1996",
  "endDate": "01 May 2025"
}
```

---

### 12. Get Deployed vs Completed Assessment Graph

**Endpoint:**

```
POST /api/v1/AnalyticalDashboard/DeployAssessGraph
```

**Payload:**

```json
{
  "startDate": "1996-02-01T00:00:00",
  "endDate": "2025-05-01T00:00:00"
}
```

**Response (example):**

```json
[
  {
    "courseId": 17070,
    "courseName": "report 1",
    "totaldeployed": 6,
    "totalcompleted": 2,
    "completionPercentage": 33.33
  },
  {
    "courseId": 17073,
    "courseName": "report 3",
    "totaldeployed": 1,
    "totalcompleted": 1,
    "completionPercentage": 100.0
  }
]
```


## 20. ILT Reports


### 1. ILT Completion Report

**Endpoint:**

```
POST /api/v1/ILTReport/ExportILTCompletionReport
```

**Payload:**

```json
{
  "startDate": "2018-02-01T16:26:34",
  "endDate": "2025-05-13T16:26:34",
  "ExportAs": "xlsx"
}
```

---

### 2. ILT Consolidated Report

**Endpoint:**

```
POST /api/v1/ILTReport/ILTConsolidatedReport
```

**Payload:**

```json
{
  "id": 54,
  "page": 1,
  "pagesize": 10,
  "fromDate": null,
  "toDate": null,
  "userStatus": null
}
```

---

### 3. Learning Report (Search by Course Name)

**Endpoint:**

```
GET /api/v1/Courses/TypeAheadReport/{courseTitle}
```

**Example:**

```
GET /api/v1/Courses/TypeAheadReport/Testing%20by%20TTSH
```

---

### 4. Export Learning Report (WNS Report)

**Endpoint:**

```
POST /api/v1/WNSReport/ExportLaLearningReport
```

**Payload:**

```json
{
  "StartDate": "2020-02-01T00:00:00",
  "EndDate": "2025-05-02T00:00:00",
  "academy": 68,
  "courseId": [54, 107],
  "coursetype": "Classroom",
  "ExportAs": "xlsx"
}
```

---

### 5. Export Schedule-wise Attendance Report

**Endpoint:**

```
POST /api/v1/ILTReport/ExportScheduleWiseAttendanceReport
```

**Payload:**

```json
{
  "courseId": 19786,
  "moduleId": 19763,
  "userId": 3573,
  "scheduleId": 2237,
  "fromDate": "2019-01-01T00:00:00.000Z",
  "toDate": "2025-05-01T00:00:00.000Z",
  "pageSize": 10,
  "ExportAs": "xlsx"
}
```

---

### 6. Get Schedule-wise Attendance Report

**Endpoint:**

```
POST /api/v1/ILTReport/GetScheduleWiseAttendanceReport
```

**Same payload as above**

---

### 7. Get Schedule-wise Attendance Report Count

**Endpoint:**

```
POST /api/v1/ILTReport/GetScheduleWiseAttendenceReport/count
```

**Same payload as above**

---

### 8. Export Attendance Summary Report

**Endpoint:**

```
POST /api/v1/Report/ExportAttendenceSummuryReport
```

**Payload:**

```json
{
  "courseId": 2264,
  "moduleId": 2404,
  "fromDate": "2018-01-01T00:00:00",
  "toDate": "2025-05-01T00:00:00",
  "startIndex": 1,
  "pageSize": 10
}
```

---

### 9. Get Attendance Summary Report

**Endpoint:**

```
POST /api/v1/Report/GetAttendenceSummuryReport
```

**Same payload as above**

---

### 10. Get Attendance Summary Report Count

**Endpoint:**

```
POST /api/v1/Report/GetAttendenceSummuryReportCount
```

**Same payload as above**

---
 20. Internal Trainers Schedule Report


### 1. Search for Internal Trainers

**Endpoint:**

```
POST /api/v1/User/GetTypeAhead
```

**Payload (example):**

```json
{
  "searchByColumn": "lbY9NRTamILZYgQ+kSRoYA==",
  "searchText": "bP654GgMMaQM9Xn9sUdrvg=="
}
```

**Note:** This is typically used to look up internal trainer details by encrypted parameters.

---

### 2. Export Internal Trainers Schedule Report

**Endpoint:**

```
POST /api/v1/ILTReport/ExportGetInternalTrainersScheduleReport
```

**Payload:**

```json
{
  "academyAgencyID": 0,
  "startDate": "2019-01-01T10:56:34.000Z",
  "endDate": "2025-05-01T10:56:34.000Z",
  "startIndex": 1,
  "pageSize": null,
  "search": null,
  "RegionID": 8,
  "count": null,
  "ExportAs": "xlsx"
}
```

## 21. Performance & Competency Management

### 21.1 Job Profiles Management
#### Get Paginated Job Roles
- **Endpoint**: `POST /api/v1/JobRolesInformation/PaginationData`
- **Authentication**: Bearer Token
- **Payload**:
```json
{"page":1, "pageSize":10, "search":null}
```
- **Response**:
```json
{
  "data": [
    {
      "id": 51,
      "jobRoleTitle": "Software Developer",
      "isActive": true
    }
  ],
  "totalRecords": 15
}
```

#### Check Implementation Scope
- **Endpoint**: `GET /api/v1/ImplementationScope`
- **Query Params**:
  - `subcategoryEnabled=true`
  - `subsetEnabled=true`
  - `levelEnabled=true`

---

### 21.2 Career Roadmap Management
#### Create Career Roadmap
- **Endpoint**: `POST /api/v1/CareerRoadmap`
- **Payload**:
```json
{
  "name": "testing",
  "description": "testing",
  "isActive": true,
  "phases": [
    {
      "jobRoleId": 51,
      "jobRoleTitle": "Software Developer",
      "jobRoleParameters": [
        {
          "mappedAttribute": "Business",
          "attributeValueName": "development"
        }
      ],
      "averageDurationInMonths": 6
    }
  ]
}
```

#### Get Career Roadmaps (Paginated)
- **Endpoint**: `GET /api/v1/CareerRoadmap/{page}/{pageSize}`
- **Response**:
```json
{
  "data": [
    {
      "id": 3,
      "name": "testing",
      "totalPhases": 1,
      "totalDurationInMonths": 6
    }
  ]
}
```

#### Get Roadmap Phases
- **Endpoint**: `GET /api/v1/CareerRoadmap/GetPhasesUnderRoadmap/{roadmapId}`
- **Response**:
```json
[
  {
    "id": 5,
    "jobRoleTitle": "Software Developer",
    "jobRoleParameters": [
      {
        "mappedAttribute": "Business",
        "attributeValueName": "development"
      }
    ]
  }
]
```

---

### 21.3 Competencies Dictionary
#### Get All Competency Categories
- **Endpoint**: `GET /api/v1/CompetencyCategory`
- **Response**:
```json
[
  {
    "id": 1,
    "categoryName": "Manager",
    "category": "Managerial Abilities"
  }
]
```

#### Create Competency Category
- **Endpoint**: `POST /api/v1/CompetencyFramework/CreateCategory`
- **Payload**:
```json
{"name": "Aarti Competency test"}
```

#### Create Competency Subcategory
- **Endpoint**: `POST /api/v1/CompetencyFramework/CreateSubcategory`
- **Payload**:
```json
{"name": "Communication Skills", "categoryId": 196}
```

#### Get Subcategories with Counts
- **Endpoint**: `GET /api/v1/CompetencyFramework/GetSubcategoriesWithSubsetCount/{categoryId}`
- **Response**:
```json
[
  {
    "subcategory": {
      "id": 52,
      "subcategoryDescription": "Communication Skills"
    },
    "subsetCount": 0
  }
]
```

---

### 21.4 Competency Review Parameters
#### Add Review Parameter
- **Endpoint**: `POST /api/v1/c/CompetencyReviewParameters`
- **Payload**:
```json
{
  "CompetencyId": 69,
  "JobRoleId": 13,
  "ReviewParameter": "Conflict resolution"
}
```

#### Get Review Parameters
- **Endpoint**: `POST /api/v1/c/CompetencyReviewParameters/getAllCompetencyReviewParameters`
- **Payload**:
```json
{"Page":1, "PageSize":10, "FilterName":null}
```

---

### 21.5 Job Description Management
#### Upload JD File
- **Endpoint**: `POST /api/v1/JobRole/PostFileUpload`
- **Content-Type**: `multipart/form-data`
- **Parameters**:
  - `fileForUpload`: JD file (PDF/DOCX)
  - `jobRoleId`: 51

#### Get All JDs
- **Endpoint**: `POST /api/v1/JobRole/GetAllJdUpload`
- **Payload**:
```json
{"page":1, "pageSize":10, "columnName":"name", "search":null}
```

#### Get JD Count
- **Endpoint**: `GET /api/v1/JobRole/GetAllJdCount`

---

### 21.6 Competency Import/Export
#### Export Competency Data
- **Endpoint**: `GET /api/v1/CompetencyCategory/Export`

#### Import Competency Data
- **Endpoint**: `POST /api/v1/CompetencyCategory/PostFileUpload`
- **Parameters**:
  - `fileForUpload`: Excel file
  - `CustomerCode`: Your org code
  - `FileType`: "xlsx"

#### Download Sample Template
- **Endpoint**: `GET /api/v1/CompetencyFramework/ExportSample`

---





### Implementation Notes:
1. All endpoints require Bearer Token authentication
2. Category/Subcategory endpoints use -1 for unlimited results



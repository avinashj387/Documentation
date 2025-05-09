# API Documentation

## Table of Contents
1. [My Courses](#my-courses)
2. [Leaderboard](#leaderboard)
3. [Explore](#explore)
4. [Knowledge Library](#knowledge-library)

---

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
      "status": "completed",
      "progressPercentage": 100,
      "thumbnailPath": "../../../assets/img/Thumbnail_vectors/img_thumb96.jpg"
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
    "courseTitle": "new deployment testing",
    "modules": [
      {
        "moduleId": 14180,
        "moduleName": "External link",
        "status": "completed"
      }
    ]
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
      "status": "completed",
      "type": "Course"
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
  ```
- **Response**: Array of ranked users
  ```json
  {
    "topRanking": [
      {
        "userName": "LMS Admin",
        "totalPoint": 29952,
        "rank": 1
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
        "userName": "Narendra Shete",
        "totalPoint": 20,
        "rank": 1
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
      "name": "Comprehensive Career Programs"
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
      "name": "Product training"
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
      "title": "gamefication_normal"
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

---

### Implementation Notes:
1. All endpoints require Bearer Token authentication
2. Category/Subcategory endpoints use -1 for unlimited results
3. Leaderboard endpoints require POST with specific payloads


---
title: Upload Microsoft Graph API 为教育作业和提交创建Graph文件
description: 了解如何使用 Microsoft Graph 中的教育 API 将文件上传到作业或提交Graph。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 0d7c60fbb88c6c6eec9f4748f2921a800f20b99e2248d6f6c26cad188591721c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54151793"
---
# <a name="upload-files-for-education-assignments-and-submissions-using-the-microsoft-graph-api"></a>Upload Microsoft Graph API 为教育作业和提交创建Graph文件

资源是教育 [作业和子](/graph/api/resources/educationassignment) 分配 [的组成部分](/graph/api/resources/educationsubmission)。 教师确定要上传到作业文件夹的资源，学生确定要上传到提交文件夹的资源。

本文介绍如何在 Microsoft Graph教育 API 将文件上载到作业或提交文件夹。

## <a name="prerequisites"></a>先决条件

在上载文件之前，请SharePoint一个文件夹，用于将给定教育作业或[子](/graph/api/resources/educationsubmission)分配资源的文件上传到该[](/graph/api/resources/educationassignment)文件夹。 

## <a name="upload-a-resource"></a>Upload资源

API `setUpResourcesFolder` 返回包含 **resourcesFolderUrl 属性** 的模型。

```http
{
    ...
    "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GFA"
    ...
}
```
以下步骤介绍如何将资源/文件上载到相关资源文件夹。

### <a name="step-1---construct-the-upload-url"></a>步骤 1 - 构造上载 URL
生成 URL 以按照此特定格式上载内容 `{resourcesFolderUrl}:/{Name of new file}:/content` 。 以下示例显示包含 **resourcesFolderUrl** 属性的上载 URL。

```http
https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2:/MyPictureFile.png:/content
```

### <a name="step-2---upload-the-resource-to-sharepoint"></a>步骤 2 - Upload资源SharePoint
使用上载 URL 提出 PUT 请求以上载内容。

请求正文的内容应该是要上载文件的二进制流。

有关详细信息，请参阅Upload[上传会话处理大型文件](/graph/api/driveitem-createuploadsession)。

#### <a name="request-example"></a>请求示例
下面为请求示例。

```http
PUT https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2:/MyPictureFile.png:/content
Content-Type: text/plain

Binary data for the file
```

#### <a name="response-example"></a>响应示例
以下示例显示了相应的响应。

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#drives('b%216SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F')/items/$entity",
    "@microsoft.graph.downloadUrl": "...",
    "createdDateTime": "2021-03-11T18:49:47Z",
    "eTag": "\"{EDD00CE7-B74C-4C3E-BA3E-484CB41EF31D},1\"",
    "id": "01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ",
    "lastModifiedDateTime": "2021-03-11T18:49:47Z",
    "name": "MyPictureFile.png",
    "webUrl": "https://contososdorg.sharepoint.com/sites/GraphTest/Class%20Files/Assignments/Test%20File%20Distribution/MyPictureFile.png",
    "cTag": "\"c:{EDD00CE7-B74C-4C3E-BA3E-484CB41EF31D},2\"",
    "size": 2302233,
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "email": "t-james@contososd.org",
            "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
            "displayName": "James"
        }
    },
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
            "email": "t-james@contososd.org",
            "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
            "displayName": "James"
        }
    },
    "parentReference": {
        "driveId": "b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F",
        "driveType": "documentLibrary",
        "id": "01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2",
        "path": "/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/root:/Assignments/Test File Distribution"
    },
    "file": {
        "mimeType": "image/png",
        "hashes": {
            "quickXorHash": "CvYQxN7MCGrIsdrA38c6wWhOu5g="
        }
    },
    "fileSystemInfo": {
        "createdDateTime": "2021-03-11T18:49:47Z",
        "lastModifiedDateTime": "2021-03-11T18:49:47Z"
    },
    "image": {}
}
```

### <a name="step-3---construct-the-value-for-the-fileurl-property"></a>步骤 3 - 构造 fileUrl 属性的值
使用下面的格式生成 **fileUrl** 属性的值 `https://graph.microsoft.com/v1.0/drives/{drive-id}/items/{item-id}` ：。 将 `{drive-id}` 和 `{item-id}` 占位符替换为下表中描述的值。

| 占位符 | 说明 | 示例 |
|:--|:--|:--|
| `{drive-id}` | 步骤 2 中使用的请求 URL 中的驱动器 ID。 | b！6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F |
| `{item-id}` | 步骤 2 中获取的响应正文中的项目 ID。 | 01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ |

下面的示例演示基于此格式的 **fileUrl。**

```http
https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ
```

### <a name="step-4---create-educationassignmentresource"></a>步骤 4 - 创建 educationAssignmentResource
此步骤演示如何将资源SharePoint工作分配资源文件夹。

使用 `fileUrl` 请求正文中上一步骤中的 创建 [educationAssignmentResource](/graph/api/educationassignment-post-resources)。

#### <a name="request-example"></a>请求示例
下面为请求示例。

```http
POST https://graph.microsoft.com/v1.0/education/classes/b07edbef-7420-4b3d-8f7c-d599cf21e069/assignments/48b80dff-452a-4108-bd85-fa0d84e39d0a/resources
Content-type: application/json

{
    "resource": {
        "@odata.type": "#microsoft.graph.educationFileResource",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ",
        "displayName": "Parts of a Sonnet"
    }
}
```

#### <a name="response-example"></a>响应示例
以下示例显示了相应的响应。

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('b07edbef-7420-4b3d-8f7c-d599cf21e069')/assignments('48b80dff-452a-4108-bd85-fa0d84e39d0a')/resources/$entity",
    "distributeForStudentWork": false,
    "id": "ff1aafe4-ae89-49c3-8366-4b509f640d6a",
    "resource": {
        "@odata.type": "#microsoft.graph.educationFileResource",
        "displayName": "Parts of a Sonnet",
        "createdDateTime": "2021-03-11T18:35:40.6642039Z",
        "lastModifiedDateTime": "2021-03-11T18:35:40.6642039Z",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
                "displayName": null
            }
        }
    }
}
```

现在，您已成功将SharePoint资源上载到工作分配资源文件夹 (并将其附加到关联的工作分配) 。 你可以按照类似的步骤上载一个或多个学生工作资源。 有关详细信息，请参阅创建 [educationSubmissionResource](/graph/api/educationsubmission-post-resources)。

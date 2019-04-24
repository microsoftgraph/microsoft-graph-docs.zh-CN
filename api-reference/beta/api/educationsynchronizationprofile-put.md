---
title: 更新 educationSynchronizationProfile
description: 更新租户中现有 school 数据同步配置文件的属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 668aad65abe2c9b3d4609400118f9341748210f1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464712"
---
# <a name="update-an-educationsynchronizationprofile"></a><span data-ttu-id="46d5a-103">更新 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="46d5a-103">Update an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46d5a-104">更新租户中现有 school 数据[同步配置文件](../resources/educationsynchronizationprofile.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="46d5a-104">Update properties for an existing school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="46d5a-105">权限</span><span class="sxs-lookup"><span data-stu-id="46d5a-105">Permissions</span></span>
<span data-ttu-id="46d5a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46d5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46d5a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="46d5a-108">Permission type</span></span> | <span data-ttu-id="46d5a-109">权限</span><span class="sxs-lookup"><span data-stu-id="46d5a-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="46d5a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46d5a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="46d5a-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46d5a-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="46d5a-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="46d5a-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="46d5a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="46d5a-113">Not supported.</span></span>|
|<span data-ttu-id="46d5a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="46d5a-114">Application</span></span>|<span data-ttu-id="46d5a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="46d5a-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46d5a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46d5a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="46d5a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="46d5a-117">Request headers</span></span>
| <span data-ttu-id="46d5a-118">名称</span><span class="sxs-lookup"><span data-stu-id="46d5a-118">Name</span></span>       | <span data-ttu-id="46d5a-119">类型</span><span class="sxs-lookup"><span data-stu-id="46d5a-119">Type</span></span> | <span data-ttu-id="46d5a-120">说明</span><span class="sxs-lookup"><span data-stu-id="46d5a-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="46d5a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="46d5a-121">Authorization</span></span>  | <span data-ttu-id="46d5a-122">string</span><span class="sxs-lookup"><span data-stu-id="46d5a-122">string</span></span>  | <span data-ttu-id="46d5a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46d5a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="46d5a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46d5a-125">Content-Type</span></span> | <span data-ttu-id="46d5a-126">string</span><span class="sxs-lookup"><span data-stu-id="46d5a-126">string</span></span> | <span data-ttu-id="46d5a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="46d5a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46d5a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="46d5a-129">Request body</span></span>
<span data-ttu-id="46d5a-130">在请求正文中, 提供[synchronizationProfile](../resources/educationsynchronizationprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46d5a-130">In the request body, supply a JSON representation of the [synchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="46d5a-131">响应</span><span class="sxs-lookup"><span data-stu-id="46d5a-131">Response</span></span>
<span data-ttu-id="46d5a-132">如果成功, 此方法在响应`202, Accepted`正文中返回响应代码和[synchronizationProfile](../resources/educationsynchronizationprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="46d5a-132">If successful, this method returns a `202, Accepted` response code and a [synchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46d5a-133">示例</span><span class="sxs-lookup"><span data-stu-id="46d5a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46d5a-134">请求</span><span class="sxs-lookup"><span data-stu-id="46d5a-134">Request</span></span>
<span data-ttu-id="46d5a-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46d5a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_synchronizationProfile"
}-->
```http
PUT https://graph.microsoft.com/beta/education/synchronizationProfiles
Content-type: application/json

{
    "displayName": "Test Profile",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationcsvdataprovider",
        "customizations": {
            "student": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Middle Name"
                ]
            }
        }
    },
    "identitySynchronizationConfiguration": {
        "@odata.type": "microsoft.graph.educationidentitycreationconfiguration",
        "userDomains": [
            {
                "appliesTo": "student",
                "name": "testschool.edu"
            },
            {
                "appliesTo": "teacher",
                "name": "testschool.edu"
            }
        ]
    },
    "licensesToAssign": [
        {
            "appliesTo": "teacher",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        },
        {
            "appliesTo": "student",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        }
    ]
}
```

##### <a name="response"></a><span data-ttu-id="46d5a-136">响应</span><span class="sxs-lookup"><span data-stu-id="46d5a-136">Response</span></span>
<span data-ttu-id="46d5a-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="46d5a-137">Here is an example of the response.</span></span> 

><span data-ttu-id="46d5a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="46d5a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "displayName": "Test Profile",
    "state": "provisioning",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationCsvDataProvider",
        "customizations": {
            "student": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Middle Name"
                ],
                "synchronizationStartDate": "0001-01-01T00:00:00Z",
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "teacher": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Teacher Number",
                    "Status",
                    "Middle Name",
                    "Secondary Email",
                    "Title",
                    "Qualification"
                ],
                "synchronizationStartDate": "0001-01-01T00:00:00Z",
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "studentEnrollment": {
                "optionalPropertiesToSync": [],
                "synchronizationStartDate": "0001-01-01T00:00:00Z",
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "teacherRoster": {
                "optionalPropertiesToSync": [],
                "synchronizationStartDate": "0001-01-01T00:00:00Z",
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            }
        }
    },
    "identitySynchronizationConfiguration": {
        "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
        "userDomains": [
            {
                "appliesTo": "student",
                "name": "testschool.edu"
            },
            {
                "appliesTo": "teacher",
                "name": "testschool.edu"
            }
        ]
    },
    "licensesToAssign": [
        {
            "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",                
            "appliesTo": "teacher",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        },
        {
            "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",                
            "appliesTo": "student",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-put.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: 更新 educationSynchronizationProfile
description: 更新为租户中为现有学校数据同步配置文件属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 07947127b0346a33528136921580646623576d28
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935085"
---
# <a name="update-an-educationsynchronizationprofile"></a><span data-ttu-id="ef6d2-103">更新 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="ef6d2-103">Update an educationSynchronizationProfile</span></span>

> <span data-ttu-id="ef6d2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ef6d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef6d2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ef6d2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef6d2-106">更新租户中的现有学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)属性。</span><span class="sxs-lookup"><span data-stu-id="ef6d2-106">Update properties for an existing school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef6d2-107">权限</span><span class="sxs-lookup"><span data-stu-id="ef6d2-107">Permissions</span></span>
<span data-ttu-id="ef6d2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef6d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef6d2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef6d2-110">Permission type</span></span> | <span data-ttu-id="ef6d2-111">权限</span><span class="sxs-lookup"><span data-stu-id="ef6d2-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ef6d2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef6d2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ef6d2-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef6d2-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="ef6d2-114">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="ef6d2-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ef6d2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef6d2-115">Not supported.</span></span>|
|<span data-ttu-id="ef6d2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef6d2-116">Application</span></span>|<span data-ttu-id="ef6d2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef6d2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef6d2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef6d2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ef6d2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef6d2-119">Request headers</span></span>
| <span data-ttu-id="ef6d2-120">名称</span><span class="sxs-lookup"><span data-stu-id="ef6d2-120">Name</span></span>       | <span data-ttu-id="ef6d2-121">类型</span><span class="sxs-lookup"><span data-stu-id="ef6d2-121">Type</span></span> | <span data-ttu-id="ef6d2-122">说明</span><span class="sxs-lookup"><span data-stu-id="ef6d2-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ef6d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef6d2-123">Authorization</span></span>  | <span data-ttu-id="ef6d2-124">string</span><span class="sxs-lookup"><span data-stu-id="ef6d2-124">string</span></span>  | <span data-ttu-id="ef6d2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ef6d2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ef6d2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef6d2-127">Content-Type</span></span> | <span data-ttu-id="ef6d2-128">string</span><span class="sxs-lookup"><span data-stu-id="ef6d2-128">string</span></span> | <span data-ttu-id="ef6d2-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ef6d2-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef6d2-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef6d2-131">Request body</span></span>
<span data-ttu-id="ef6d2-132">在请求正文中，提供[synchronizationProfile](../resources/educationsynchronizationprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef6d2-132">In the request body, supply a JSON representation of the [synchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ef6d2-133">响应</span><span class="sxs-lookup"><span data-stu-id="ef6d2-133">Response</span></span>
<span data-ttu-id="ef6d2-134">如果成功，此方法返回`202, Accepted`响应代码和响应正文中的[synchronizationProfile](../resources/educationsynchronizationprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ef6d2-134">If successful, this method returns a `202, Accepted` response code and a [synchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef6d2-135">示例</span><span class="sxs-lookup"><span data-stu-id="ef6d2-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef6d2-136">请求</span><span class="sxs-lookup"><span data-stu-id="ef6d2-136">Request</span></span>
<span data-ttu-id="ef6d2-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ef6d2-137">Here is an example of the request.</span></span>
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
        "@odata.type": "#microsoft.graph.educationcsvdataprovider",
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
        "@odata.type": "#microsoft.graph.educationidentitycreationconfiguration",
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

##### <a name="response"></a><span data-ttu-id="ef6d2-138">响应</span><span class="sxs-lookup"><span data-stu-id="ef6d2-138">Response</span></span>
<span data-ttu-id="ef6d2-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ef6d2-139">Here is an example of the response.</span></span> 

><span data-ttu-id="ef6d2-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ef6d2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "displayName": "Test Profile",
    "state": "provisioning",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "dataProvider": {
        "@odata.type": "#microsoft.graph.educationCsvDataProvider",
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
        "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
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
            "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment",                
            "appliesTo": "teacher",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        },
        {
            "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment",                
            "appliesTo": "student",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        }
    ]
}
```

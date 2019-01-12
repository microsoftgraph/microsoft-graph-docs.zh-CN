---
title: 创建 educationSynchronizationProfile
description: '在租户中创建一个新的学校数据同步配置文件的请求。 查询以获取配置文件的状态的状态。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9d471766a8492e03809d05d6d0366c8e44d59015
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915758"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="864cc-104">创建 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="864cc-104">Create an educationSynchronizationProfile</span></span>

> <span data-ttu-id="864cc-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="864cc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="864cc-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="864cc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="864cc-107">在租户中创建新的学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的请求。</span><span class="sxs-lookup"><span data-stu-id="864cc-107">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="864cc-108">[查询状态](educationsynchronizationprofilestatus-get.md)，以获取配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="864cc-108">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="864cc-109">权限</span><span class="sxs-lookup"><span data-stu-id="864cc-109">Permissions</span></span>
<span data-ttu-id="864cc-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="864cc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="864cc-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="864cc-112">Permission type</span></span> | <span data-ttu-id="864cc-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="864cc-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="864cc-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="864cc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="864cc-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="864cc-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="864cc-116">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="864cc-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="864cc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="864cc-117">Not supported.</span></span>|
|<span data-ttu-id="864cc-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="864cc-118">Application</span></span>|<span data-ttu-id="864cc-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="864cc-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="864cc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="864cc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="864cc-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="864cc-121">Request headers</span></span>
| <span data-ttu-id="864cc-122">名称</span><span class="sxs-lookup"><span data-stu-id="864cc-122">Name</span></span>       | <span data-ttu-id="864cc-123">类型</span><span class="sxs-lookup"><span data-stu-id="864cc-123">Type</span></span> | <span data-ttu-id="864cc-124">说明</span><span class="sxs-lookup"><span data-stu-id="864cc-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="864cc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="864cc-125">Authorization</span></span>  | <span data-ttu-id="864cc-126">string</span><span class="sxs-lookup"><span data-stu-id="864cc-126">string</span></span>  | <span data-ttu-id="864cc-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="864cc-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="864cc-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="864cc-129">Content-Type</span></span> | <span data-ttu-id="864cc-130">string</span><span class="sxs-lookup"><span data-stu-id="864cc-130">string</span></span> | <span data-ttu-id="864cc-131">应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="864cc-131">Application/json.</span></span> <span data-ttu-id="864cc-132">必填。</span><span class="sxs-lookup"><span data-stu-id="864cc-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="864cc-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="864cc-133">Request body</span></span>
<span data-ttu-id="864cc-134">在请求正文中，提供[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="864cc-134">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="864cc-135">响应</span><span class="sxs-lookup"><span data-stu-id="864cc-135">Response</span></span>
<span data-ttu-id="864cc-136">如果成功，此方法返回`202, Accepted`响应代码和响应正文中的[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="864cc-136">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="864cc-137">示例</span><span class="sxs-lookup"><span data-stu-id="864cc-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="864cc-138">请求</span><span class="sxs-lookup"><span data-stu-id="864cc-138">Request</span></span>
<span data-ttu-id="864cc-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="864cc-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationSynchronizationProfile"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles
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

##### <a name="response"></a><span data-ttu-id="864cc-140">响应</span><span class="sxs-lookup"><span data-stu-id="864cc-140">Response</span></span>
<span data-ttu-id="864cc-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="864cc-141">The following is an example of the response.</span></span> 

><span data-ttu-id="864cc-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="864cc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 201 Created
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

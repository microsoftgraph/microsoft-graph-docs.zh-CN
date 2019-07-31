---
title: 创建 educationSynchronizationProfile
description: '在租户中创建新的学校数据同步配置文件的请求。 查询状态以获取配置文件的状态。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e4fe25723d146a30ad94bd99491bafe293da523a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954807"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="2a38d-104">创建 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="2a38d-104">Create an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a38d-105">在租户中创建新的学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的请求。</span><span class="sxs-lookup"><span data-stu-id="2a38d-105">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="2a38d-106">[查询状态](educationsynchronizationprofilestatus-get.md)以获取配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="2a38d-106">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2a38d-107">权限</span><span class="sxs-lookup"><span data-stu-id="2a38d-107">Permissions</span></span>
<span data-ttu-id="2a38d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a38d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a38d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a38d-110">Permission type</span></span> | <span data-ttu-id="2a38d-111">权限</span><span class="sxs-lookup"><span data-stu-id="2a38d-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="2a38d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a38d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2a38d-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a38d-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="2a38d-114">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="2a38d-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2a38d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a38d-115">Not supported.</span></span>|
|<span data-ttu-id="2a38d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a38d-116">Application</span></span>|<span data-ttu-id="2a38d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a38d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a38d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a38d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="2a38d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a38d-119">Request headers</span></span>
| <span data-ttu-id="2a38d-120">名称</span><span class="sxs-lookup"><span data-stu-id="2a38d-120">Name</span></span>       | <span data-ttu-id="2a38d-121">类型</span><span class="sxs-lookup"><span data-stu-id="2a38d-121">Type</span></span> | <span data-ttu-id="2a38d-122">说明</span><span class="sxs-lookup"><span data-stu-id="2a38d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2a38d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a38d-123">Authorization</span></span>  | <span data-ttu-id="2a38d-124">string</span><span class="sxs-lookup"><span data-stu-id="2a38d-124">string</span></span>  | <span data-ttu-id="2a38d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2a38d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2a38d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a38d-127">Content-Type</span></span> | <span data-ttu-id="2a38d-128">string</span><span class="sxs-lookup"><span data-stu-id="2a38d-128">string</span></span> | <span data-ttu-id="2a38d-129">Application/json。</span><span class="sxs-lookup"><span data-stu-id="2a38d-129">Application/json.</span></span> <span data-ttu-id="2a38d-130">必需。</span><span class="sxs-lookup"><span data-stu-id="2a38d-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a38d-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a38d-131">Request body</span></span>
<span data-ttu-id="2a38d-132">在请求正文中, 提供[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a38d-132">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2a38d-133">响应</span><span class="sxs-lookup"><span data-stu-id="2a38d-133">Response</span></span>
<span data-ttu-id="2a38d-134">如果成功, 此方法在响应`202, Accepted`正文中返回响应代码和[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2a38d-134">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a38d-135">示例</span><span class="sxs-lookup"><span data-stu-id="2a38d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a38d-136">请求</span><span class="sxs-lookup"><span data-stu-id="2a38d-136">Request</span></span>
<span data-ttu-id="2a38d-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2a38d-137">The following is an example of the request.</span></span>
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
        "@odata.type": "microsoft.graph.educationCsvDataProvider",
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
        "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration",
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

##### <a name="response"></a><span data-ttu-id="2a38d-138">响应</span><span class="sxs-lookup"><span data-stu-id="2a38d-138">Response</span></span>
<span data-ttu-id="2a38d-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2a38d-139">The following is an example of the response.</span></span> 

><span data-ttu-id="2a38d-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2a38d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 201 Created
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

---
title: 创建 educationSynchronizationProfile
description: '在租户中创建新的学校数据同步配置文件的请求。 查询状态，获取配置文件的状态。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e55a24642f6b29ce280775f779f005fd76d4996c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043071"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="c1841-104">创建 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="c1841-104">Create an educationSynchronizationProfile</span></span>

<span data-ttu-id="c1841-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1841-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1841-106">在租户中创建新的学校数据 [同步](../resources/educationsynchronizationprofile.md) 配置文件的请求。</span><span class="sxs-lookup"><span data-stu-id="c1841-106">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="c1841-107">[查询状态](educationsynchronizationprofilestatus-get.md) ，获取配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="c1841-107">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c1841-108">权限</span><span class="sxs-lookup"><span data-stu-id="c1841-108">Permissions</span></span>
<span data-ttu-id="c1841-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1841-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1841-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1841-111">Permission type</span></span> | <span data-ttu-id="c1841-112">权限</span><span class="sxs-lookup"><span data-stu-id="c1841-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c1841-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1841-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c1841-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1841-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="c1841-115">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="c1841-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c1841-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1841-116">Not supported.</span></span>|
|<span data-ttu-id="c1841-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1841-117">Application</span></span>|<span data-ttu-id="c1841-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1841-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1841-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1841-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="c1841-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1841-120">Request headers</span></span>
| <span data-ttu-id="c1841-121">名称</span><span class="sxs-lookup"><span data-stu-id="c1841-121">Name</span></span>       | <span data-ttu-id="c1841-122">类型</span><span class="sxs-lookup"><span data-stu-id="c1841-122">Type</span></span> | <span data-ttu-id="c1841-123">说明</span><span class="sxs-lookup"><span data-stu-id="c1841-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c1841-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1841-124">Authorization</span></span>  | <span data-ttu-id="c1841-125">string</span><span class="sxs-lookup"><span data-stu-id="c1841-125">string</span></span>  | <span data-ttu-id="c1841-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1841-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c1841-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1841-128">Content-Type</span></span> | <span data-ttu-id="c1841-129">string</span><span class="sxs-lookup"><span data-stu-id="c1841-129">string</span></span> | <span data-ttu-id="c1841-130">Application/json。</span><span class="sxs-lookup"><span data-stu-id="c1841-130">Application/json.</span></span> <span data-ttu-id="c1841-131">必需。</span><span class="sxs-lookup"><span data-stu-id="c1841-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1841-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1841-132">Request body</span></span>
<span data-ttu-id="c1841-133">在请求正文中，提供 [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1841-133">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c1841-134">响应</span><span class="sxs-lookup"><span data-stu-id="c1841-134">Response</span></span>
<span data-ttu-id="c1841-135">如果成功，此方法在响应正文中返回 响应代码和 `202, Accepted` [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1841-135">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1841-136">示例</span><span class="sxs-lookup"><span data-stu-id="c1841-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1841-137">请求</span><span class="sxs-lookup"><span data-stu-id="c1841-137">Request</span></span>
<span data-ttu-id="c1841-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1841-138">The following is an example of the request.</span></span>
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
        "@odata.type": "#Microsoft.Education.DataSync.educationCsvDataProvider",
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
        "@odata.type": "#Microsoft.Education.DataSync.educationIdentityCreationConfiguration",
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

##### <a name="response"></a><span data-ttu-id="c1841-139">响应</span><span class="sxs-lookup"><span data-stu-id="c1841-139">Response</span></span>
<span data-ttu-id="c1841-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1841-140">The following is an example of the response.</span></span> 

><span data-ttu-id="c1841-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c1841-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
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



---
title: 获取 educationSynchronizationProfile
description: 根据标识符检索租户中的学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 52d40288237b417138d7ad54a290fc4529f3e10f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954857"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="96d8c-103">获取 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="96d8c-103">Get an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96d8c-104">根据标识符检索租户中的学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="96d8c-104">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="96d8c-105">权限</span><span class="sxs-lookup"><span data-stu-id="96d8c-105">Permissions</span></span>
<span data-ttu-id="96d8c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96d8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96d8c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="96d8c-108">Permission type</span></span> | <span data-ttu-id="96d8c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96d8c-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="96d8c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96d8c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96d8c-111">EduAdministration、EduAdministration</span><span class="sxs-lookup"><span data-stu-id="96d8c-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="96d8c-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="96d8c-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="96d8c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="96d8c-113">Not supported.</span></span>|
|<span data-ttu-id="96d8c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="96d8c-114">Application</span></span>| <span data-ttu-id="96d8c-115">EduAdministration、EduAdministration 和所有</span><span class="sxs-lookup"><span data-stu-id="96d8c-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96d8c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96d8c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="96d8c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="96d8c-117">Request headers</span></span>
| <span data-ttu-id="96d8c-118">名称</span><span class="sxs-lookup"><span data-stu-id="96d8c-118">Name</span></span>       | <span data-ttu-id="96d8c-119">类型</span><span class="sxs-lookup"><span data-stu-id="96d8c-119">Type</span></span> | <span data-ttu-id="96d8c-120">说明</span><span class="sxs-lookup"><span data-stu-id="96d8c-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="96d8c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="96d8c-121">Authorization</span></span>  | <span data-ttu-id="96d8c-122">string</span><span class="sxs-lookup"><span data-stu-id="96d8c-122">string</span></span>  | <span data-ttu-id="96d8c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96d8c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96d8c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="96d8c-125">Request body</span></span>
<span data-ttu-id="96d8c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96d8c-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="96d8c-127">响应</span><span class="sxs-lookup"><span data-stu-id="96d8c-127">Response</span></span>
<span data-ttu-id="96d8c-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="96d8c-128">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96d8c-129">示例</span><span class="sxs-lookup"><span data-stu-id="96d8c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96d8c-130">请求</span><span class="sxs-lookup"><span data-stu-id="96d8c-130">Request</span></span>
<span data-ttu-id="96d8c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="96d8c-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationSynchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="96d8c-132">响应</span><span class="sxs-lookup"><span data-stu-id="96d8c-132">Response</span></span>
<span data-ttu-id="96d8c-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="96d8c-133">The following is an example of the response.</span></span> 

><span data-ttu-id="96d8c-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="96d8c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2487

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/$entity",
    "displayName": "Test Profile",
    "state": "provisioned",
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
    "licensesToAssign": 
         [
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

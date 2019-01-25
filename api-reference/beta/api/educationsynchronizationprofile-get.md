---
title: 获取 educationSynchronizationProfile
description: 检索学校数据同步配置文件中租户基于的标识符。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 47757956db9e93bb13f4167ef330c7b79d7851b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530179"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="e49bd-103">获取 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="e49bd-103">Get an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e49bd-104">检索基于标识符为租户中学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="e49bd-104">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="e49bd-105">权限</span><span class="sxs-lookup"><span data-stu-id="e49bd-105">Permissions</span></span>
<span data-ttu-id="e49bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e49bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e49bd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e49bd-108">Permission type</span></span> | <span data-ttu-id="e49bd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e49bd-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="e49bd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e49bd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e49bd-111">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e49bd-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="e49bd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e49bd-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e49bd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e49bd-113">Not supported.</span></span>|
|<span data-ttu-id="e49bd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e49bd-114">Application</span></span>| <span data-ttu-id="e49bd-115">EduAdministration.Read.All EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e49bd-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e49bd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e49bd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e49bd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e49bd-117">Request headers</span></span>
| <span data-ttu-id="e49bd-118">名称</span><span class="sxs-lookup"><span data-stu-id="e49bd-118">Name</span></span>       | <span data-ttu-id="e49bd-119">类型</span><span class="sxs-lookup"><span data-stu-id="e49bd-119">Type</span></span> | <span data-ttu-id="e49bd-120">说明</span><span class="sxs-lookup"><span data-stu-id="e49bd-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e49bd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e49bd-121">Authorization</span></span>  | <span data-ttu-id="e49bd-122">string</span><span class="sxs-lookup"><span data-stu-id="e49bd-122">string</span></span>  | <span data-ttu-id="e49bd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e49bd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e49bd-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e49bd-125">Request body</span></span>
<span data-ttu-id="e49bd-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e49bd-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e49bd-127">响应</span><span class="sxs-lookup"><span data-stu-id="e49bd-127">Response</span></span>
<span data-ttu-id="e49bd-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e49bd-128">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e49bd-129">示例</span><span class="sxs-lookup"><span data-stu-id="e49bd-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e49bd-130">请求</span><span class="sxs-lookup"><span data-stu-id="e49bd-130">Request</span></span>
<span data-ttu-id="e49bd-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e49bd-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationSynchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="e49bd-132">响应</span><span class="sxs-lookup"><span data-stu-id="e49bd-132">Response</span></span>
<span data-ttu-id="e49bd-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e49bd-133">The following is an example of the response.</span></span> 

><span data-ttu-id="e49bd-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e49bd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: 列表 educationSynchronizationProfiles
description: 检索为租户中的学校数据同步配置文件的集合。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1907b0ef08473a79d66e79fcb4751b281e9a18ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509551"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="650a0-103">列表 educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="650a0-103">List educationSynchronizationProfiles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="650a0-104">检索为租户中的学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="650a0-104">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="650a0-105">权限</span><span class="sxs-lookup"><span data-stu-id="650a0-105">Permissions</span></span>
<span data-ttu-id="650a0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="650a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="650a0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="650a0-108">Permission type</span></span> | <span data-ttu-id="650a0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="650a0-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="650a0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="650a0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="650a0-111">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="650a0-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="650a0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="650a0-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="650a0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="650a0-113">Not supported.</span></span>|
|<span data-ttu-id="650a0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="650a0-114">Application</span></span>|<span data-ttu-id="650a0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="650a0-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="650a0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="650a0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="650a0-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="650a0-117">Optional query parameters</span></span>
<span data-ttu-id="650a0-118">此方法支持以下[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)以帮助自定义响应： $filter、 $orderby、 $top、 $skip 和 $count。</span><span class="sxs-lookup"><span data-stu-id="650a0-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="650a0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="650a0-119">Request headers</span></span>
| <span data-ttu-id="650a0-120">名称</span><span class="sxs-lookup"><span data-stu-id="650a0-120">Name</span></span>       | <span data-ttu-id="650a0-121">类型</span><span class="sxs-lookup"><span data-stu-id="650a0-121">Type</span></span> | <span data-ttu-id="650a0-122">说明</span><span class="sxs-lookup"><span data-stu-id="650a0-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="650a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="650a0-123">Authorization</span></span>  | <span data-ttu-id="650a0-124">string</span><span class="sxs-lookup"><span data-stu-id="650a0-124">string</span></span>  | <span data-ttu-id="650a0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="650a0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="650a0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="650a0-127">Request body</span></span>
<span data-ttu-id="650a0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="650a0-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="650a0-129">响应</span><span class="sxs-lookup"><span data-stu-id="650a0-129">Response</span></span>
<span data-ttu-id="650a0-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="650a0-130">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="650a0-131">示例</span><span class="sxs-lookup"><span data-stu-id="650a0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="650a0-132">请求</span><span class="sxs-lookup"><span data-stu-id="650a0-132">Request</span></span>
<span data-ttu-id="650a0-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="650a0-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "list_synchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

##### <a name="response"></a><span data-ttu-id="650a0-134">响应</span><span class="sxs-lookup"><span data-stu-id="650a0-134">Response</span></span>
<span data-ttu-id="650a0-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="650a0-135">The following is an example of the response.</span></span> 

><span data-ttu-id="650a0-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="650a0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3296

{
    "value": [
    {
        "displayName": "Test Profile",
        "state": "provisioned",
        "id": "15e9b9fa-de85-492e-aa44-550c40de626e",
        "dataProvider": {
            "@odata.type": "microsoft.graph.educationCsvDataProvider",
            "customizations": {
                "school": {
                    "optionalPropertiesToSync": [
                        "School NCES_ID",
                        "State ID",
                        "GradeLow",
                        "GradeHigh",
                        "Principal Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "section": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "student": {
                    "optionalPropertiesToSync": [
                        "State ID",
                        "Email",
                        "Middle Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "teacher": {
                    "optionalPropertiesToSync": [
                        "Teacher Number",
                        "Middle Name"
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
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

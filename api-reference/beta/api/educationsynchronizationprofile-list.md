---
title: 列出 educationSynchronizationProfiles
description: 检索租户中的学校数据同步配置文件的集合。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ee295989618b4095425267fd1ff3d0bebfaf8baf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954860"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="19041-103">列出 educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="19041-103">List educationSynchronizationProfiles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19041-104">检索租户中的学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="19041-104">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="19041-105">权限</span><span class="sxs-lookup"><span data-stu-id="19041-105">Permissions</span></span>
<span data-ttu-id="19041-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19041-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19041-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="19041-108">Permission type</span></span> | <span data-ttu-id="19041-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19041-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="19041-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19041-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19041-111">EduAdministration、EduAdministration</span><span class="sxs-lookup"><span data-stu-id="19041-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="19041-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="19041-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="19041-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="19041-113">Not supported.</span></span>|
|<span data-ttu-id="19041-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="19041-114">Application</span></span>|<span data-ttu-id="19041-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="19041-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19041-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19041-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19041-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="19041-117">Optional query parameters</span></span>
<span data-ttu-id="19041-118">此方法支持以下[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters), 以帮助自定义响应: $filter、$orderby、$top、$skip 和 $count。</span><span class="sxs-lookup"><span data-stu-id="19041-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19041-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="19041-119">Request headers</span></span>
| <span data-ttu-id="19041-120">名称</span><span class="sxs-lookup"><span data-stu-id="19041-120">Name</span></span>       | <span data-ttu-id="19041-121">类型</span><span class="sxs-lookup"><span data-stu-id="19041-121">Type</span></span> | <span data-ttu-id="19041-122">说明</span><span class="sxs-lookup"><span data-stu-id="19041-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="19041-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19041-123">Authorization</span></span>  | <span data-ttu-id="19041-124">string</span><span class="sxs-lookup"><span data-stu-id="19041-124">string</span></span>  | <span data-ttu-id="19041-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19041-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="19041-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="19041-127">Request body</span></span>
<span data-ttu-id="19041-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="19041-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="19041-129">响应</span><span class="sxs-lookup"><span data-stu-id="19041-129">Response</span></span>
<span data-ttu-id="19041-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="19041-130">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19041-131">示例</span><span class="sxs-lookup"><span data-stu-id="19041-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19041-132">请求</span><span class="sxs-lookup"><span data-stu-id="19041-132">Request</span></span>
<span data-ttu-id="19041-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="19041-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "list_synchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

##### <a name="response"></a><span data-ttu-id="19041-134">响应</span><span class="sxs-lookup"><span data-stu-id="19041-134">Response</span></span>
<span data-ttu-id="19041-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="19041-135">The following is an example of the response.</span></span> 

><span data-ttu-id="19041-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="19041-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

---
title: 列出 educationSynchronizationProfiles
description: 检索租户中学校数据同步配置文件的集合。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: bb4996140bc0ec7200bedb4243f4eef0f10f080d
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664746"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="84286-103">列出 educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="84286-103">List educationSynchronizationProfiles</span></span>

<span data-ttu-id="84286-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84286-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84286-105">检索租户中学校 [数据同步](../resources/educationsynchronizationprofile.md) 配置文件的集合。</span><span class="sxs-lookup"><span data-stu-id="84286-105">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="84286-106">权限</span><span class="sxs-lookup"><span data-stu-id="84286-106">Permissions</span></span>
<span data-ttu-id="84286-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84286-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84286-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="84286-109">Permission type</span></span> | <span data-ttu-id="84286-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84286-110">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="84286-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84286-111">Delegated (work or school account)</span></span> | <span data-ttu-id="84286-112">EduAdministration.Read、EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84286-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="84286-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="84286-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="84286-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="84286-114">Not supported.</span></span>|
|<span data-ttu-id="84286-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="84286-115">Application</span></span>|<span data-ttu-id="84286-116">EduAdministration.Read.All、EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84286-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84286-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84286-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84286-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="84286-118">Optional query parameters</span></span>
<span data-ttu-id="84286-119">此方法支持以下 [OData](/graph/query-parameters) 查询参数来帮助自定义响应：$filter、$orderby、$top、$skip 和 $count。</span><span class="sxs-lookup"><span data-stu-id="84286-119">This method supports the following [OData Query Parameters](/graph/query-parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84286-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="84286-120">Request headers</span></span>
| <span data-ttu-id="84286-121">名称</span><span class="sxs-lookup"><span data-stu-id="84286-121">Name</span></span>       | <span data-ttu-id="84286-122">类型</span><span class="sxs-lookup"><span data-stu-id="84286-122">Type</span></span> | <span data-ttu-id="84286-123">说明</span><span class="sxs-lookup"><span data-stu-id="84286-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="84286-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="84286-124">Authorization</span></span>  | <span data-ttu-id="84286-125">string</span><span class="sxs-lookup"><span data-stu-id="84286-125">string</span></span>  | <span data-ttu-id="84286-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84286-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="84286-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="84286-128">Request body</span></span>
<span data-ttu-id="84286-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="84286-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="84286-130">响应</span><span class="sxs-lookup"><span data-stu-id="84286-130">Response</span></span>
<span data-ttu-id="84286-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="84286-131">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84286-132">示例</span><span class="sxs-lookup"><span data-stu-id="84286-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84286-133">请求</span><span class="sxs-lookup"><span data-stu-id="84286-133">Request</span></span>
<span data-ttu-id="84286-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="84286-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84286-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="84286-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_synchronizationProfile"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```
# <a name="c"></a>[<span data-ttu-id="84286-136">C#</span><span class="sxs-lookup"><span data-stu-id="84286-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84286-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84286-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84286-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84286-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84286-139">Java</span><span class="sxs-lookup"><span data-stu-id="84286-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-synchronizationprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="84286-140">响应</span><span class="sxs-lookup"><span data-stu-id="84286-140">Response</span></span>
<span data-ttu-id="84286-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="84286-141">The following is an example of the response.</span></span> 

><span data-ttu-id="84286-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="84286-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
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

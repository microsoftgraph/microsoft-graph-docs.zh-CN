---
title: 获取 educationSynchronizationErrors
description: '获取在验证过程中生成的错误和/或在租户中同步特定学校数据同步配置文件的过程。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8f2f3076ca757ef941087e0334583246d0543856
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720303"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="1ee6c-103">获取 educationSynchronizationErrors</span><span class="sxs-lookup"><span data-stu-id="1ee6c-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="1ee6c-104">获取在验证过程中生成的错误和/或在租户中同步特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的过程。</span><span class="sxs-lookup"><span data-stu-id="1ee6c-104">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> 

## <a name="permissions"></a><span data-ttu-id="1ee6c-105">权限</span><span class="sxs-lookup"><span data-stu-id="1ee6c-105">Permissions</span></span>
<span data-ttu-id="1ee6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ee6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ee6c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ee6c-108">Permission type</span></span> | <span data-ttu-id="1ee6c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ee6c-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:------|
| <span data-ttu-id="1ee6c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ee6c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1ee6c-111">EduAdministration、EduAdministration</span><span class="sxs-lookup"><span data-stu-id="1ee6c-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="1ee6c-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="1ee6c-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="1ee6c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ee6c-113">Not supported.</span></span>|
|<span data-ttu-id="1ee6c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ee6c-114">Application</span></span>| <span data-ttu-id="1ee6c-115">EduAdministration、EduAdministration 和所有</span><span class="sxs-lookup"><span data-stu-id="1ee6c-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ee6c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ee6c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/errors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1ee6c-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1ee6c-117">Optional query parameters</span></span>
<span data-ttu-id="1ee6c-118">此方法支持以下[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters), 以帮助自定义响应: $filter、$orderby、$top、$skip 和 $count。</span><span class="sxs-lookup"><span data-stu-id="1ee6c-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ee6c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ee6c-119">Request headers</span></span>
| <span data-ttu-id="1ee6c-120">名称</span><span class="sxs-lookup"><span data-stu-id="1ee6c-120">Name</span></span>       | <span data-ttu-id="1ee6c-121">类型</span><span class="sxs-lookup"><span data-stu-id="1ee6c-121">Type</span></span> | <span data-ttu-id="1ee6c-122">说明</span><span class="sxs-lookup"><span data-stu-id="1ee6c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1ee6c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ee6c-123">Authorization</span></span>  | <span data-ttu-id="1ee6c-124">string</span><span class="sxs-lookup"><span data-stu-id="1ee6c-124">string</span></span>  | <span data-ttu-id="1ee6c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ee6c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1ee6c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ee6c-127">Request body</span></span>
<span data-ttu-id="1ee6c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ee6c-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1ee6c-129">响应</span><span class="sxs-lookup"><span data-stu-id="1ee6c-129">Response</span></span>
<span data-ttu-id="1ee6c-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[同步错误](../resources/educationsynchronizationerror.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="1ee6c-130">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ee6c-131">示例</span><span class="sxs-lookup"><span data-stu-id="1ee6c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ee6c-132">请求</span><span class="sxs-lookup"><span data-stu-id="1ee6c-132">Request</span></span>
<span data-ttu-id="1ee6c-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1ee6c-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1ee6c-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1ee6c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1ee6c-135">C#</span><span class="sxs-lookup"><span data-stu-id="1ee6c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ee6c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ee6c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1ee6c-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="1ee6c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1ee6c-138">响应</span><span class="sxs-lookup"><span data-stu-id="1ee6c-138">Response</span></span>
<span data-ttu-id="1ee6c-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1ee6c-139">The following is an example of the response.</span></span> 

><span data-ttu-id="1ee6c-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1ee6c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationError",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1568

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/errors",
    "@odata.count": 14,
    "value": [
        {
            "entryType": "Student",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Student cannot be updated as no matching entry in Active Directory was found for Student.  Verify the identity matching criteria for the profile.",
            "joiningValue": "richard.2wilson@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:45Z",
            "reportableIdentifier": "richard.2wilson"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "alberto2.dorsey@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "alberto2.dorsey"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "madeline2.bullock@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "madeline2.bullock"
        }
    ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

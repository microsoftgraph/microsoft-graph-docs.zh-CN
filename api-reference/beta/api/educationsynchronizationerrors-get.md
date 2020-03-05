---
title: 获取 educationSynchronizationErrors
description: '获取在验证过程中生成的错误和/或在租户中同步特定学校数据同步配置文件的过程。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 81da0a081976e97254b541c0d4d07e13ed51c854
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424608"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="72fee-103">获取 educationSynchronizationErrors</span><span class="sxs-lookup"><span data-stu-id="72fee-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="72fee-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="72fee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72fee-105">获取在验证过程中生成的错误和/或在租户中同步特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的过程。</span><span class="sxs-lookup"><span data-stu-id="72fee-105">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> 

## <a name="permissions"></a><span data-ttu-id="72fee-106">权限</span><span class="sxs-lookup"><span data-stu-id="72fee-106">Permissions</span></span>
<span data-ttu-id="72fee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72fee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72fee-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="72fee-109">Permission type</span></span> | <span data-ttu-id="72fee-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72fee-110">Permissions (from least to most privileged)</span></span> |
|:-----------|:------|
| <span data-ttu-id="72fee-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72fee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="72fee-112">EduAdministration、EduAdministration</span><span class="sxs-lookup"><span data-stu-id="72fee-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="72fee-113">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="72fee-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="72fee-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="72fee-114">Not supported.</span></span>|
|<span data-ttu-id="72fee-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="72fee-115">Application</span></span>| <span data-ttu-id="72fee-116">EduAdministration、EduAdministration 和所有</span><span class="sxs-lookup"><span data-stu-id="72fee-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72fee-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72fee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/errors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="72fee-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="72fee-118">Optional query parameters</span></span>
<span data-ttu-id="72fee-119">此方法支持以下[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)，以帮助自定义响应： $filter、$orderby、$top、$skip 和 $count。</span><span class="sxs-lookup"><span data-stu-id="72fee-119">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72fee-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="72fee-120">Request headers</span></span>
| <span data-ttu-id="72fee-121">名称</span><span class="sxs-lookup"><span data-stu-id="72fee-121">Name</span></span>       | <span data-ttu-id="72fee-122">类型</span><span class="sxs-lookup"><span data-stu-id="72fee-122">Type</span></span> | <span data-ttu-id="72fee-123">说明</span><span class="sxs-lookup"><span data-stu-id="72fee-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="72fee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="72fee-124">Authorization</span></span>  | <span data-ttu-id="72fee-125">string</span><span class="sxs-lookup"><span data-stu-id="72fee-125">string</span></span>  | <span data-ttu-id="72fee-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="72fee-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="72fee-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="72fee-128">Request body</span></span>
<span data-ttu-id="72fee-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="72fee-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="72fee-130">响应</span><span class="sxs-lookup"><span data-stu-id="72fee-130">Response</span></span>
<span data-ttu-id="72fee-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[同步错误](../resources/educationsynchronizationerror.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="72fee-131">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72fee-132">示例</span><span class="sxs-lookup"><span data-stu-id="72fee-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72fee-133">请求</span><span class="sxs-lookup"><span data-stu-id="72fee-133">Request</span></span>
<span data-ttu-id="72fee-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="72fee-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72fee-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="72fee-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```
# <a name="c"></a>[<span data-ttu-id="72fee-136">C#</span><span class="sxs-lookup"><span data-stu-id="72fee-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72fee-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72fee-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72fee-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72fee-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="72fee-139">响应</span><span class="sxs-lookup"><span data-stu-id="72fee-139">Response</span></span>
<span data-ttu-id="72fee-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="72fee-140">The following is an example of the response.</span></span> 

><span data-ttu-id="72fee-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="72fee-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/errors",
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

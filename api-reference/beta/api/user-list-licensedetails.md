---
title: List licenseDetails
description: 检索 licenseDetails 对象的列表。
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: c35bc0faec06d61aac67c5be2570e344d3e884e9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036280"
---
# <a name="list-licensedetails"></a><span data-ttu-id="cf00e-103">List licenseDetails</span><span class="sxs-lookup"><span data-stu-id="cf00e-103">List licenseDetails</span></span>

<span data-ttu-id="cf00e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf00e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf00e-105">检索企业用户的 **licenseDetails** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="cf00e-105">Retrieve a list of **licenseDetails** objects for enterprise users.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf00e-106">权限</span><span class="sxs-lookup"><span data-stu-id="cf00e-106">Permissions</span></span>
<span data-ttu-id="cf00e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf00e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf00e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf00e-109">Permission type</span></span>      | <span data-ttu-id="cf00e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf00e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf00e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf00e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cf00e-112">User.Read、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cf00e-112">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cf00e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf00e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf00e-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="cf00e-114">User.Read</span></span>    |
|<span data-ttu-id="cf00e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf00e-115">Application</span></span> | <span data-ttu-id="cf00e-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf00e-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf00e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf00e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cf00e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cf00e-118">Optional query parameters</span></span>
<span data-ttu-id="cf00e-119">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="cf00e-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="cf00e-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="cf00e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf00e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf00e-121">Request headers</span></span>
| <span data-ttu-id="cf00e-122">名称</span><span class="sxs-lookup"><span data-stu-id="cf00e-122">Name</span></span>      |<span data-ttu-id="cf00e-123">说明</span><span class="sxs-lookup"><span data-stu-id="cf00e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cf00e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf00e-124">Authorization</span></span>  | <span data-ttu-id="cf00e-125">Bearer &lt; code&gt;</span><span class="sxs-lookup"><span data-stu-id="cf00e-125">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf00e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf00e-126">Request body</span></span>
<span data-ttu-id="cf00e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf00e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf00e-128">响应</span><span class="sxs-lookup"><span data-stu-id="cf00e-128">Response</span></span>

<span data-ttu-id="cf00e-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [licenseDetails](../resources/licensedetails.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cf00e-129">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf00e-130">示例</span><span class="sxs-lookup"><span data-stu-id="cf00e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf00e-131">请求</span><span class="sxs-lookup"><span data-stu-id="cf00e-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cf00e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf00e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/licenseDetails
```
# <a name="c"></a>[<span data-ttu-id="cf00e-133">C#</span><span class="sxs-lookup"><span data-stu-id="cf00e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-licensedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf00e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf00e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-licensedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf00e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf00e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-licensedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf00e-136">Java</span><span class="sxs-lookup"><span data-stu-id="cf00e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-licensedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cf00e-137">响应</span><span class="sxs-lookup"><span data-stu-id="cf00e-137">Response</span></span>
<span data-ttu-id="cf00e-138">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cf00e-138">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



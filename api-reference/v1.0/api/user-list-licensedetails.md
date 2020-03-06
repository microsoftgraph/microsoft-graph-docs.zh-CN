---
title: List licenseDetails
description: 检索 licenseDetails 对象的列表。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0ff8d83748d8a285011b078abc028826d026125f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509085"
---
# <a name="list-licensedetails"></a><span data-ttu-id="2ea37-103">List licenseDetails</span><span class="sxs-lookup"><span data-stu-id="2ea37-103">List licenseDetails</span></span>

<span data-ttu-id="2ea37-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ea37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2ea37-105">检索 licenseDetails 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="2ea37-105">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ea37-106">权限</span><span class="sxs-lookup"><span data-stu-id="2ea37-106">Permissions</span></span>
<span data-ttu-id="2ea37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ea37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ea37-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ea37-109">Permission type</span></span>      | <span data-ttu-id="2ea37-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ea37-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ea37-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ea37-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ea37-112">User. read，User. all，All，all，Directory.accessasuser.all，all，all，all，all。 All</span><span class="sxs-lookup"><span data-stu-id="2ea37-112">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2ea37-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ea37-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ea37-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="2ea37-114">User.Read</span></span>    |
|<span data-ttu-id="2ea37-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ea37-115">Application</span></span> | <span data-ttu-id="2ea37-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ea37-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ea37-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ea37-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2ea37-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2ea37-118">Optional query parameters</span></span>
<span data-ttu-id="2ea37-119">此方法**不**支持[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="2ea37-119">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ea37-120">请求头</span><span class="sxs-lookup"><span data-stu-id="2ea37-120">Request headers</span></span>
| <span data-ttu-id="2ea37-121">名称</span><span class="sxs-lookup"><span data-stu-id="2ea37-121">Name</span></span>      |<span data-ttu-id="2ea37-122">说明</span><span class="sxs-lookup"><span data-stu-id="2ea37-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2ea37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ea37-123">Authorization</span></span>  | <span data-ttu-id="2ea37-124">持有&lt;者代码&gt;</span><span class="sxs-lookup"><span data-stu-id="2ea37-124">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ea37-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ea37-125">Request body</span></span>
<span data-ttu-id="2ea37-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ea37-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ea37-127">响应</span><span class="sxs-lookup"><span data-stu-id="2ea37-127">Response</span></span>

<span data-ttu-id="2ea37-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[licenseDetails](../resources/licensedetails.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="2ea37-128">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2ea37-129">示例</span><span class="sxs-lookup"><span data-stu-id="2ea37-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ea37-130">请求</span><span class="sxs-lookup"><span data-stu-id="2ea37-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2ea37-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ea37-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
# <a name="c"></a>[<span data-ttu-id="2ea37-132">C#</span><span class="sxs-lookup"><span data-stu-id="2ea37-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-licensedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ea37-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ea37-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-licensedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ea37-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ea37-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-licensedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ea37-135">Java</span><span class="sxs-lookup"><span data-stu-id="2ea37-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-licensedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2ea37-136">响应</span><span class="sxs-lookup"><span data-stu-id="2ea37-136">Response</span></span>
<span data-ttu-id="2ea37-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2ea37-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

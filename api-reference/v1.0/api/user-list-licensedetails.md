---
title: List licenseDetails
description: 检索 licenseDetails 对象的列表。
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: c0c4f0cebd430b0087f295a5ae4ecd0b92904512
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719925"
---
# <a name="list-licensedetails"></a><span data-ttu-id="4ba92-103">List licenseDetails</span><span class="sxs-lookup"><span data-stu-id="4ba92-103">List licenseDetails</span></span>

<span data-ttu-id="4ba92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ba92-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ba92-105">检索企业用户的 **licenseDetails** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="4ba92-105">Retrieve a list of **licenseDetails** objects for enterprise users.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ba92-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4ba92-106">Permissions</span></span>
<span data-ttu-id="4ba92-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ba92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ba92-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ba92-109">Permission type</span></span>      | <span data-ttu-id="4ba92-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ba92-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ba92-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ba92-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ba92-112">User.Read、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4ba92-112">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4ba92-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ba92-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ba92-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="4ba92-114">User.Read</span></span>    |
|<span data-ttu-id="4ba92-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ba92-115">Application</span></span> | <span data-ttu-id="4ba92-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ba92-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ba92-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ba92-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ba92-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4ba92-118">Optional query parameters</span></span>
<span data-ttu-id="4ba92-119">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="4ba92-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="4ba92-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="4ba92-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ba92-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ba92-121">Request headers</span></span>
| <span data-ttu-id="4ba92-122">名称</span><span class="sxs-lookup"><span data-stu-id="4ba92-122">Name</span></span>      |<span data-ttu-id="4ba92-123">说明</span><span class="sxs-lookup"><span data-stu-id="4ba92-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4ba92-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ba92-124">Authorization</span></span>  | <span data-ttu-id="4ba92-125">Bearer &lt; code&gt;</span><span class="sxs-lookup"><span data-stu-id="4ba92-125">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ba92-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ba92-126">Request body</span></span>
<span data-ttu-id="4ba92-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ba92-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ba92-128">响应</span><span class="sxs-lookup"><span data-stu-id="4ba92-128">Response</span></span>

<span data-ttu-id="4ba92-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [licenseDetails](../resources/licensedetails.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4ba92-129">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ba92-130">示例</span><span class="sxs-lookup"><span data-stu-id="4ba92-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ba92-131">请求</span><span class="sxs-lookup"><span data-stu-id="4ba92-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4ba92-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ba92-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
# <a name="c"></a>[<span data-ttu-id="4ba92-133">C#</span><span class="sxs-lookup"><span data-stu-id="4ba92-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-licensedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ba92-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ba92-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-licensedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ba92-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ba92-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-licensedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ba92-136">Java</span><span class="sxs-lookup"><span data-stu-id="4ba92-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-licensedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4ba92-137">响应</span><span class="sxs-lookup"><span data-stu-id="4ba92-137">Response</span></span>
<span data-ttu-id="4ba92-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ba92-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


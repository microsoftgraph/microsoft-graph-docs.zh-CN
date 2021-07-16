---
title: 获取 termStore 组
description: 读取 group 对象的属性和关系。
author: mohitpcad
localization_priority: Normal
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: 8f36e8b6b2e03ed9a05294b35736dbbb1b0dd578
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2021
ms.locfileid: "53458965"
---
# <a name="get-termstore-group"></a><span data-ttu-id="b19c1-103">获取 termStore 组</span><span class="sxs-lookup"><span data-stu-id="b19c1-103">Get termStore group</span></span>
<span data-ttu-id="b19c1-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="b19c1-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b19c1-105">读取术语库组对象的属性 [和](../resources/termstore-group.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="b19c1-105">Read the properties and relationships of a term store [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b19c1-106">权限</span><span class="sxs-lookup"><span data-stu-id="b19c1-106">Permissions</span></span>
<span data-ttu-id="b19c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b19c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b19c1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b19c1-109">Permission type</span></span>|<span data-ttu-id="b19c1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b19c1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b19c1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b19c1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b19c1-112">TermStore.Read.All、TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b19c1-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="b19c1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b19c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b19c1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b19c1-114">Not supported.</span></span>    |
|<span data-ttu-id="b19c1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b19c1-115">Application</span></span> | <span data-ttu-id="b19c1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b19c1-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="b19c1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b19c1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{group-id}
GET /sites/{site-id}/termStore/groups/{group-id}
```

## <a name="request-headers"></a><span data-ttu-id="b19c1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b19c1-118">Request headers</span></span>
|<span data-ttu-id="b19c1-119">名称</span><span class="sxs-lookup"><span data-stu-id="b19c1-119">Name</span></span>|<span data-ttu-id="b19c1-120">说明</span><span class="sxs-lookup"><span data-stu-id="b19c1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b19c1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b19c1-121">Authorization</span></span>|<span data-ttu-id="b19c1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b19c1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b19c1-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b19c1-124">Request body</span></span>
<span data-ttu-id="b19c1-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b19c1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b19c1-126">响应</span><span class="sxs-lookup"><span data-stu-id="b19c1-126">Response</span></span>

<span data-ttu-id="b19c1-127">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [microsoft.graph.termStore.group](../resources/termstore-group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b19c1-127">If successful, this method returns a `200 OK` response code and a [microsoft.graph.termStore.group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b19c1-128">示例</span><span class="sxs-lookup"><span data-stu-id="b19c1-128">Examples</span></span>

### <a name="example-1-get-a-termstore-group"></a><span data-ttu-id="b19c1-129">示例 1：获取 termStore 组</span><span class="sxs-lookup"><span data-stu-id="b19c1-129">Example 1: Get a termStore group</span></span>

#### <a name="request"></a><span data-ttu-id="b19c1-130">请求</span><span class="sxs-lookup"><span data-stu-id="b19c1-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b19c1-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b19c1-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C
```
# <a name="c"></a>[<span data-ttu-id="b19c1-132">C#</span><span class="sxs-lookup"><span data-stu-id="b19c1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b19c1-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b19c1-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b19c1-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b19c1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b19c1-135">Java</span><span class="sxs-lookup"><span data-stu-id="b19c1-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b19c1-136">响应</span><span class="sxs-lookup"><span data-stu-id="b19c1-136">Response</span></span>

><span data-ttu-id="b19c1-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b19c1-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "id": "1FFD3F87-9464-488A-A0EC-8FB90911182C",
  "displayName": "myGroup"  
}
```
### <a name="example-2-get-a-termstore-group-and-its-parent-site-id"></a><span data-ttu-id="b19c1-138">示例 2：获取 termStore 组及其父网站 ID</span><span class="sxs-lookup"><span data-stu-id="b19c1-138">Example 2: Get a termStore group and its parent site ID</span></span>

#### <a name="request"></a><span data-ttu-id="b19c1-139">请求</span><span class="sxs-lookup"><span data-stu-id="b19c1-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b19c1-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b19c1-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C?$select=*,parentSiteId
```
# <a name="c"></a>[<span data-ttu-id="b19c1-141">C#</span><span class="sxs-lookup"><span data-stu-id="b19c1-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b19c1-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b19c1-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b19c1-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b19c1-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b19c1-144">Java</span><span class="sxs-lookup"><span data-stu-id="b19c1-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b19c1-145">响应</span><span class="sxs-lookup"><span data-stu-id="b19c1-145">Response</span></span>

><span data-ttu-id="b19c1-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b19c1-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "id": "1FFD3F87-9464-488A-A0EC-8FB90911182C",
  "displayName": "myGroup",
  "parentSiteId": "microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f"
}
```

### <a name="example-3-get-a-site-collection-termstore-group"></a><span data-ttu-id="b19c1-147">示例 3：获取网站集术语存储组</span><span class="sxs-lookup"><span data-stu-id="b19c1-147">Example 3: Get a site collection termStore group</span></span>
#### <a name="request"></a><span data-ttu-id="b19c1-148">请求</span><span class="sxs-lookup"><span data-stu-id="b19c1-148">Request</span></span>


<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C
```

#### <a name="response"></a><span data-ttu-id="b19c1-149">响应</span><span class="sxs-lookup"><span data-stu-id="b19c1-149">Response</span></span>

><span data-ttu-id="b19c1-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b19c1-150">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "id": "1FFD3F87-9464-488A-A0EC-8FB90911182C",
  "displayName": "myGroup",
}
```

[microsoft.graph.termStore.store]: ../resources/termstore-store.md
[microsoft.graph.termStore.group]: ../resources/termstore-group.md

<!--
{
  "type": "#page.annotation",
  "description": "Get termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termGroup",
  "suppressions": [
  ]
}
-->



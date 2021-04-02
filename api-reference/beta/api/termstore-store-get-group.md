---
title: 获取组
description: 读取 group 对象的属性和关系。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2c95937181d90a2f1b8759464b7ef8506397c4a1
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507163"
---
# <a name="get-group"></a><span data-ttu-id="13c1b-103">获取组</span><span class="sxs-lookup"><span data-stu-id="13c1b-103">Get group</span></span>
<span data-ttu-id="13c1b-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="13c1b-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13c1b-105">读取术语库组对象的属性 [和](../resources/termstore-group.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="13c1b-105">Read the properties and relationships of a term store [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="13c1b-106">权限</span><span class="sxs-lookup"><span data-stu-id="13c1b-106">Permissions</span></span>
<span data-ttu-id="13c1b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13c1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13c1b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="13c1b-109">Permission type</span></span>|<span data-ttu-id="13c1b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13c1b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13c1b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13c1b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="13c1b-112">TermStore.Read.All、TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c1b-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="13c1b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13c1b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13c1b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="13c1b-114">Not supported.</span></span>    |
|<span data-ttu-id="13c1b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="13c1b-115">Application</span></span> | <span data-ttu-id="13c1b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="13c1b-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="13c1b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13c1b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="13c1b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="13c1b-118">Request headers</span></span>
|<span data-ttu-id="13c1b-119">名称</span><span class="sxs-lookup"><span data-stu-id="13c1b-119">Name</span></span>|<span data-ttu-id="13c1b-120">说明</span><span class="sxs-lookup"><span data-stu-id="13c1b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="13c1b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="13c1b-121">Authorization</span></span>|<span data-ttu-id="13c1b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="13c1b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="13c1b-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="13c1b-124">Request body</span></span>
<span data-ttu-id="13c1b-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="13c1b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13c1b-126">响应</span><span class="sxs-lookup"><span data-stu-id="13c1b-126">Response</span></span>

<span data-ttu-id="13c1b-127">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [microsoft.graph.termStore.group](../resources/termstore-group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="13c1b-127">If successful, this method returns a `200 OK` response code and a [microsoft.graph.termStore.group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13c1b-128">示例</span><span class="sxs-lookup"><span data-stu-id="13c1b-128">Examples</span></span>

### <a name="example-1-get-a-termstore-group"></a><span data-ttu-id="13c1b-129">示例 1：获取 termStore 组</span><span class="sxs-lookup"><span data-stu-id="13c1b-129">Example 1: Get a termStore group</span></span>

#### <a name="request"></a><span data-ttu-id="13c1b-130">请求</span><span class="sxs-lookup"><span data-stu-id="13c1b-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="13c1b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="13c1b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}
```
# <a name="c"></a>[<span data-ttu-id="13c1b-132">C#</span><span class="sxs-lookup"><span data-stu-id="13c1b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13c1b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13c1b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13c1b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13c1b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13c1b-135">Java</span><span class="sxs-lookup"><span data-stu-id="13c1b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="13c1b-136">响应</span><span class="sxs-lookup"><span data-stu-id="13c1b-136">Response</span></span>

<span data-ttu-id="13c1b-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="13c1b-137">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-2-get-a-termstore-group-and-its-parent-site-id"></a><span data-ttu-id="13c1b-138">示例 2：获取 termStore 组及其父网站 ID</span><span class="sxs-lookup"><span data-stu-id="13c1b-138">Example 2: Get a termStore group and its parent site ID</span></span>

#### <a name="request"></a><span data-ttu-id="13c1b-139">请求</span><span class="sxs-lookup"><span data-stu-id="13c1b-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="13c1b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="13c1b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}?$select=*,parentSiteId
```
# <a name="c"></a>[<span data-ttu-id="13c1b-141">C#</span><span class="sxs-lookup"><span data-stu-id="13c1b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13c1b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13c1b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13c1b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13c1b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13c1b-144">Java</span><span class="sxs-lookup"><span data-stu-id="13c1b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="13c1b-145">响应</span><span class="sxs-lookup"><span data-stu-id="13c1b-145">Response</span></span>

<span data-ttu-id="13c1b-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="13c1b-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "parentSiteId": "microsoft.sharepoint.com,05259ba9-25a8-4c93-a9a9-f995ef1fc51f,a785ad58-1d57-4f8a-aa71-77170459bd0d"
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



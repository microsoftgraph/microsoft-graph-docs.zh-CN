---
title: 获取组
description: 读取 group 对象的属性和关系。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: ef7eae93b2906467b8bbfafc0a2b48b0a07f4cc3
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874128"
---
# <a name="get-group"></a><span data-ttu-id="30bd1-103">获取组</span><span class="sxs-lookup"><span data-stu-id="30bd1-103">Get group</span></span>
<span data-ttu-id="30bd1-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="30bd1-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30bd1-105">读取 group [对象的属性和](../resources/termstore-group.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="30bd1-105">Read the properties and relationships of a [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="30bd1-106">权限</span><span class="sxs-lookup"><span data-stu-id="30bd1-106">Permissions</span></span>
<span data-ttu-id="30bd1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30bd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30bd1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="30bd1-109">Permission type</span></span>|<span data-ttu-id="30bd1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30bd1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30bd1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30bd1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="30bd1-112">TermStore.Read.All、TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30bd1-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="30bd1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30bd1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30bd1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="30bd1-114">Not supported.</span></span>    |
|<span data-ttu-id="30bd1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="30bd1-115">Application</span></span> | <span data-ttu-id="30bd1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="30bd1-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="30bd1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30bd1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="30bd1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="30bd1-118">Request headers</span></span>
|<span data-ttu-id="30bd1-119">名称</span><span class="sxs-lookup"><span data-stu-id="30bd1-119">Name</span></span>|<span data-ttu-id="30bd1-120">说明</span><span class="sxs-lookup"><span data-stu-id="30bd1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="30bd1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="30bd1-121">Authorization</span></span>|<span data-ttu-id="30bd1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="30bd1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30bd1-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="30bd1-124">Request body</span></span>
<span data-ttu-id="30bd1-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="30bd1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30bd1-126">响应</span><span class="sxs-lookup"><span data-stu-id="30bd1-126">Response</span></span>

<span data-ttu-id="30bd1-127">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [group](../resources/termstore-group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="30bd1-127">If successful, this method returns a `200 OK` response code and a [group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="30bd1-128">示例</span><span class="sxs-lookup"><span data-stu-id="30bd1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="30bd1-129">请求</span><span class="sxs-lookup"><span data-stu-id="30bd1-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="30bd1-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="30bd1-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}
```
# <a name="c"></a>[<span data-ttu-id="30bd1-131">C#</span><span class="sxs-lookup"><span data-stu-id="30bd1-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30bd1-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30bd1-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30bd1-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30bd1-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30bd1-134">Java</span><span class="sxs-lookup"><span data-stu-id="30bd1-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="30bd1-135">响应</span><span class="sxs-lookup"><span data-stu-id="30bd1-135">Response</span></span>

<span data-ttu-id="30bd1-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="30bd1-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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



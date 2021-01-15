---
title: 获取应用商店
description: 读取 store 对象的属性和关系。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: fb94dd40644fc1c8ad3f1727fa41b9143f2b1e13
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874415"
---
# <a name="get-store"></a><span data-ttu-id="b7d0d-103">获取应用商店</span><span class="sxs-lookup"><span data-stu-id="b7d0d-103">Get store</span></span>
<span data-ttu-id="b7d0d-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="b7d0d-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7d0d-105">读取 store [对象的属性和](../resources/termstore-store.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="b7d0d-105">Read the properties and relationships of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7d0d-106">权限</span><span class="sxs-lookup"><span data-stu-id="b7d0d-106">Permissions</span></span>
<span data-ttu-id="b7d0d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7d0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7d0d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7d0d-109">Permission type</span></span>|<span data-ttu-id="b7d0d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7d0d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7d0d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7d0d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b7d0d-112">TermStore.Read.All、TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7d0d-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="b7d0d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7d0d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7d0d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7d0d-114">Not supported.</span></span>    |
|<span data-ttu-id="b7d0d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7d0d-115">Application</span></span> | <span data-ttu-id="b7d0d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7d0d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7d0d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7d0d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore
```

## <a name="request-headers"></a><span data-ttu-id="b7d0d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7d0d-118">Request headers</span></span>
|<span data-ttu-id="b7d0d-119">名称</span><span class="sxs-lookup"><span data-stu-id="b7d0d-119">Name</span></span>|<span data-ttu-id="b7d0d-120">说明</span><span class="sxs-lookup"><span data-stu-id="b7d0d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b7d0d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7d0d-121">Authorization</span></span>|<span data-ttu-id="b7d0d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b7d0d-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="b7d0d-124">响应</span><span class="sxs-lookup"><span data-stu-id="b7d0d-124">Response</span></span>

<span data-ttu-id="b7d0d-125">如果成功，此方法在响应 `200 OK` 正文中返回响应代码[](../resources/termstore-store.md)和存储对象。</span><span class="sxs-lookup"><span data-stu-id="b7d0d-125">If successful, this method returns a `200 OK` response code and a [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7d0d-126">示例</span><span class="sxs-lookup"><span data-stu-id="b7d0d-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7d0d-127">请求</span><span class="sxs-lookup"><span data-stu-id="b7d0d-127">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b7d0d-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7d0d-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_store"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore
```
# <a name="c"></a>[<span data-ttu-id="b7d0d-129">C#</span><span class="sxs-lookup"><span data-stu-id="b7d0d-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7d0d-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7d0d-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7d0d-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7d0d-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b7d0d-132">Java</span><span class="sxs-lookup"><span data-stu-id="b7d0d-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-store-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b7d0d-133">响应</span><span class="sxs-lookup"><span data-stu-id="b7d0d-133">Response</span></span>
<span data-ttu-id="b7d0d-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b7d0d-134">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.store"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{  
  "id": "dad13b4b-3b4b-dad1-4b3b-d1da4b3bd1da",
  "defaultLanguageTag" : "en-US",
  "languageTags" : ["en-US", "de-DE", "fr-FR"]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get termStore entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termStore",
  "suppressions": []
}
-->



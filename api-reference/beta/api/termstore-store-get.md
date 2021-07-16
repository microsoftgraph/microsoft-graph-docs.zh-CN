---
title: 获取应用商店
description: 读取 store 对象的属性和关系。
author: mohitpcad
localization_priority: Normal
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: 71f23420196bab347cfe74068602b128eada36f4
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456483"
---
# <a name="get-store"></a><span data-ttu-id="52b6b-103">获取应用商店</span><span class="sxs-lookup"><span data-stu-id="52b6b-103">Get store</span></span>
<span data-ttu-id="52b6b-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="52b6b-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52b6b-105">读取 store [对象的属性和](../resources/termstore-store.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="52b6b-105">Read the properties and relationships of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="52b6b-106">权限</span><span class="sxs-lookup"><span data-stu-id="52b6b-106">Permissions</span></span>
<span data-ttu-id="52b6b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="52b6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52b6b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="52b6b-109">Permission type</span></span>|<span data-ttu-id="52b6b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="52b6b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52b6b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52b6b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="52b6b-112">TermStore.Read.All、TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52b6b-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="52b6b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52b6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52b6b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="52b6b-114">Not supported.</span></span>    |
|<span data-ttu-id="52b6b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="52b6b-115">Application</span></span> | <span data-ttu-id="52b6b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="52b6b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52b6b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52b6b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore
GET /sites/{site-id}/termStore
```

## <a name="request-headers"></a><span data-ttu-id="52b6b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="52b6b-118">Request headers</span></span>
|<span data-ttu-id="52b6b-119">名称</span><span class="sxs-lookup"><span data-stu-id="52b6b-119">Name</span></span>|<span data-ttu-id="52b6b-120">说明</span><span class="sxs-lookup"><span data-stu-id="52b6b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="52b6b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="52b6b-121">Authorization</span></span>|<span data-ttu-id="52b6b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="52b6b-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="52b6b-124">响应</span><span class="sxs-lookup"><span data-stu-id="52b6b-124">Response</span></span>

<span data-ttu-id="52b6b-125">如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/termstore-store.md) 代码和 store 对象。</span><span class="sxs-lookup"><span data-stu-id="52b6b-125">If successful, this method returns a `200 OK` response code and a [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52b6b-126">示例</span><span class="sxs-lookup"><span data-stu-id="52b6b-126">Examples</span></span>

### <a name="example-1-get-a-termstore"></a><span data-ttu-id="52b6b-127">示例 1：获取 termStore</span><span class="sxs-lookup"><span data-stu-id="52b6b-127">Example 1: Get a termStore</span></span>

#### <a name="request"></a><span data-ttu-id="52b6b-128">请求</span><span class="sxs-lookup"><span data-stu-id="52b6b-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="52b6b-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="52b6b-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_store"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore
```
# <a name="c"></a>[<span data-ttu-id="52b6b-130">C#</span><span class="sxs-lookup"><span data-stu-id="52b6b-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52b6b-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52b6b-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52b6b-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52b6b-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52b6b-133">Java</span><span class="sxs-lookup"><span data-stu-id="52b6b-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-store-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="52b6b-134">响应</span><span class="sxs-lookup"><span data-stu-id="52b6b-134">Response</span></span>
><span data-ttu-id="52b6b-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="52b6b-135">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-a-site-collection-termstore"></a><span data-ttu-id="52b6b-136">示例 2：获取网站集术语Store</span><span class="sxs-lookup"><span data-stu-id="52b6b-136">Example 2: Get a site collection termStore</span></span>

#### <a name="request"></a><span data-ttu-id="52b6b-137">请求</span><span class="sxs-lookup"><span data-stu-id="52b6b-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_store"
}-->

``` http
GET https://graph.microsoft.com/beta/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore
```

#### <a name="response"></a><span data-ttu-id="52b6b-138">响应</span><span class="sxs-lookup"><span data-stu-id="52b6b-138">Response</span></span>
><span data-ttu-id="52b6b-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="52b6b-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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



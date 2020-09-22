---
title: 获取存储区
description: 读取 store 对象的属性和关系。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 78d0482a3427874af55d2788e3e7b56b40a80cd7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044268"
---
# <a name="get-store"></a><span data-ttu-id="d28fe-103">获取存储区</span><span class="sxs-lookup"><span data-stu-id="d28fe-103">Get store</span></span>
<span data-ttu-id="d28fe-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="d28fe-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d28fe-105">读取 [store](../resources/termstore-store.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d28fe-105">Read the properties and relationships of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d28fe-106">权限</span><span class="sxs-lookup"><span data-stu-id="d28fe-106">Permissions</span></span>
<span data-ttu-id="d28fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d28fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d28fe-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d28fe-109">Permission type</span></span>|<span data-ttu-id="d28fe-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d28fe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d28fe-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d28fe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d28fe-112">TermStore、TermStore 和所有</span><span class="sxs-lookup"><span data-stu-id="d28fe-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d28fe-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d28fe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d28fe-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d28fe-114">Not supported.</span></span>    |
|<span data-ttu-id="d28fe-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d28fe-115">Application</span></span> | <span data-ttu-id="d28fe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d28fe-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d28fe-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d28fe-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore
```

## <a name="request-headers"></a><span data-ttu-id="d28fe-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d28fe-118">Request headers</span></span>
|<span data-ttu-id="d28fe-119">名称</span><span class="sxs-lookup"><span data-stu-id="d28fe-119">Name</span></span>|<span data-ttu-id="d28fe-120">说明</span><span class="sxs-lookup"><span data-stu-id="d28fe-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d28fe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d28fe-121">Authorization</span></span>|<span data-ttu-id="d28fe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d28fe-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="d28fe-124">响应</span><span class="sxs-lookup"><span data-stu-id="d28fe-124">Response</span></span>

<span data-ttu-id="d28fe-125">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [store](../resources/termstore-store.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d28fe-125">If successful, this method returns a `200 OK` response code and a [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d28fe-126">示例</span><span class="sxs-lookup"><span data-stu-id="d28fe-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d28fe-127">请求</span><span class="sxs-lookup"><span data-stu-id="d28fe-127">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d28fe-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="d28fe-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_store"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore
```
# <a name="c"></a>[<span data-ttu-id="d28fe-129">C#</span><span class="sxs-lookup"><span data-stu-id="d28fe-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d28fe-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d28fe-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d28fe-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d28fe-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d28fe-132">响应</span><span class="sxs-lookup"><span data-stu-id="d28fe-132">Response</span></span>
<span data-ttu-id="d28fe-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d28fe-133">**Note:** The response object shown here might be shortened for readability.</span></span>

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



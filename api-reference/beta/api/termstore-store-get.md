---
title: 获取存储区
description: 读取 store 对象的属性和关系。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 05175c566aa3c9ea516b9c5126754c0dce348571
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972340"
---
# <a name="get-store"></a><span data-ttu-id="94da0-103">获取存储区</span><span class="sxs-lookup"><span data-stu-id="94da0-103">Get store</span></span>
<span data-ttu-id="94da0-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="94da0-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94da0-105">读取 [store](../resources/termstore-store.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94da0-105">Read the properties and relationships of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="94da0-106">权限</span><span class="sxs-lookup"><span data-stu-id="94da0-106">Permissions</span></span>
<span data-ttu-id="94da0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94da0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94da0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="94da0-109">Permission type</span></span>|<span data-ttu-id="94da0-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="94da0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94da0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94da0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="94da0-112">TermStore、TermStore 和所有</span><span class="sxs-lookup"><span data-stu-id="94da0-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="94da0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94da0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94da0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="94da0-114">Not supported.</span></span>    |
|<span data-ttu-id="94da0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="94da0-115">Application</span></span> | <span data-ttu-id="94da0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="94da0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94da0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94da0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore
```

## <a name="request-headers"></a><span data-ttu-id="94da0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="94da0-118">Request headers</span></span>
|<span data-ttu-id="94da0-119">名称</span><span class="sxs-lookup"><span data-stu-id="94da0-119">Name</span></span>|<span data-ttu-id="94da0-120">说明</span><span class="sxs-lookup"><span data-stu-id="94da0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="94da0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="94da0-121">Authorization</span></span>|<span data-ttu-id="94da0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94da0-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="94da0-124">响应</span><span class="sxs-lookup"><span data-stu-id="94da0-124">Response</span></span>

<span data-ttu-id="94da0-125">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [store](../resources/termstore-store.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94da0-125">If successful, this method returns a `200 OK` response code and a [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94da0-126">示例</span><span class="sxs-lookup"><span data-stu-id="94da0-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94da0-127">请求</span><span class="sxs-lookup"><span data-stu-id="94da0-127">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="94da0-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="94da0-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_store"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore
```
# <a name="c"></a>[<span data-ttu-id="94da0-129">C#</span><span class="sxs-lookup"><span data-stu-id="94da0-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94da0-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94da0-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94da0-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94da0-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94da0-132">Java</span><span class="sxs-lookup"><span data-stu-id="94da0-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-store-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="94da0-133">响应</span><span class="sxs-lookup"><span data-stu-id="94da0-133">Response</span></span>
<span data-ttu-id="94da0-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="94da0-134">**Note:** The response object shown here might be shortened for readability.</span></span>

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



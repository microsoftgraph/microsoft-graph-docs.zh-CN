---
title: 更新存储
description: 更新存储对象的属性。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 73d1fb22b92c134fc4ebb2b15fe4b9314dce2d5d
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874100"
---
# <a name="update-store"></a><span data-ttu-id="d4dce-103">更新存储</span><span class="sxs-lookup"><span data-stu-id="d4dce-103">Update store</span></span>
<span data-ttu-id="d4dce-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="d4dce-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4dce-105">更新 [存储对象的属性](../resources/termstore-store.md) 。</span><span class="sxs-lookup"><span data-stu-id="d4dce-105">Update the properties of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4dce-106">权限</span><span class="sxs-lookup"><span data-stu-id="d4dce-106">Permissions</span></span>
<span data-ttu-id="d4dce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4dce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4dce-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4dce-109">Permission type</span></span>|<span data-ttu-id="d4dce-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4dce-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4dce-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4dce-111">Delegated (work or school account)</span></span> |<span data-ttu-id="d4dce-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4dce-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d4dce-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4dce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4dce-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4dce-114">Not supported.</span></span>    |
|<span data-ttu-id="d4dce-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4dce-115">Application</span></span> | <span data-ttu-id="d4dce-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4dce-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4dce-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4dce-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

``` http
PATCH /termStore
```

## <a name="request-headers"></a><span data-ttu-id="d4dce-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4dce-118">Request headers</span></span>
|<span data-ttu-id="d4dce-119">名称</span><span class="sxs-lookup"><span data-stu-id="d4dce-119">Name</span></span>|<span data-ttu-id="d4dce-120">说明</span><span class="sxs-lookup"><span data-stu-id="d4dce-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d4dce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4dce-121">Authorization</span></span>|<span data-ttu-id="d4dce-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d4dce-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d4dce-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4dce-124">Content-Type</span></span>|<span data-ttu-id="d4dce-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d4dce-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4dce-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4dce-127">Request body</span></span>
<span data-ttu-id="d4dce-128">在请求正文中，提供存储对象的 JSON [表示](../resources/termstore-store.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="d4dce-128">In the request body, supply a JSON representation of the [store](../resources/termstore-store.md) object.</span></span>

<span data-ttu-id="d4dce-129">下表显示了可编辑应用商店 [的属性](../resources/termstore-store.md)。</span><span class="sxs-lookup"><span data-stu-id="d4dce-129">The following table shows the properties that can be edited for the [store](../resources/termstore-store.md).</span></span>

|<span data-ttu-id="d4dce-130">属性</span><span class="sxs-lookup"><span data-stu-id="d4dce-130">Property</span></span>|<span data-ttu-id="d4dce-131">类型</span><span class="sxs-lookup"><span data-stu-id="d4dce-131">Type</span></span>|<span data-ttu-id="d4dce-132">Description</span><span class="sxs-lookup"><span data-stu-id="d4dce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4dce-133">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="d4dce-133">defaultLanguageTag</span></span>|<span data-ttu-id="d4dce-134">String</span><span class="sxs-lookup"><span data-stu-id="d4dce-134">String</span></span>|<span data-ttu-id="d4dce-135">[microsoft.graph.termstore.store 的默认语言](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="d4dce-135">Default language of the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|
|<span data-ttu-id="d4dce-136">languageTags</span><span class="sxs-lookup"><span data-stu-id="d4dce-136">languageTags</span></span>|<span data-ttu-id="d4dce-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="d4dce-137">String collection</span></span>|<span data-ttu-id="d4dce-138">[microsoft.graph.termstore.store 中的可用语言](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="d4dce-138">Available languages in the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d4dce-139">响应</span><span class="sxs-lookup"><span data-stu-id="d4dce-139">Response</span></span>

<span data-ttu-id="d4dce-140">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和更新[](../resources/termstore-store.md)的存储区对象。</span><span class="sxs-lookup"><span data-stu-id="d4dce-140">If successful, this method returns a `200 OK` response code and an updated [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4dce-141">示例</span><span class="sxs-lookup"><span data-stu-id="d4dce-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4dce-142">请求</span><span class="sxs-lookup"><span data-stu-id="d4dce-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d4dce-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4dce-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_store"
} -->

``` http
PATCH https://graph.microsoft.com/beta/termStore
Content-Type: application/json
Content-length: 133

{
  "defaultLanguageTag": "en-US"
}
```
# <a name="javascript"></a>[<span data-ttu-id="d4dce-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4dce-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4dce-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4dce-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="d4dce-146">C#</span><span class="sxs-lookup"><span data-stu-id="d4dce-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4dce-147">Java</span><span class="sxs-lookup"><span data-stu-id="d4dce-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-store-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d4dce-148">响应</span><span class="sxs-lookup"><span data-stu-id="d4dce-148">Response</span></span>
<span data-ttu-id="d4dce-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d4dce-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "defaultLanguageTag": "en-US",
  "languageTags": [
    "en-US", 
    "fr-FR"
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Update termstore",
  "suppressions": [
  ]
}
-->




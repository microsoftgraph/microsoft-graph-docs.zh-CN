---
title: 更新集
description: 更新 set 对象的属性。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: fe2b221bc6e6852af5d8aadcf283e851e1c47872
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872056"
---
# <a name="update-set"></a><span data-ttu-id="f5c5e-103">更新集</span><span class="sxs-lookup"><span data-stu-id="f5c5e-103">Update set</span></span>
<span data-ttu-id="f5c5e-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="f5c5e-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5c5e-105">更新 set [对象的属性](../resources/termstore-set.md) 。</span><span class="sxs-lookup"><span data-stu-id="f5c5e-105">Update the properties of a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5c5e-106">权限</span><span class="sxs-lookup"><span data-stu-id="f5c5e-106">Permissions</span></span>
<span data-ttu-id="f5c5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5c5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5c5e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5c5e-109">Permission type</span></span>|<span data-ttu-id="f5c5e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5c5e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5c5e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5c5e-111">Delegated (work or school account)</span></span> |<span data-ttu-id="f5c5e-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5c5e-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="f5c5e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5c5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5c5e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5c5e-114">Not supported.</span></span>    |
|<span data-ttu-id="f5c5e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5c5e-115">Application</span></span> | <span data-ttu-id="f5c5e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5c5e-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="f5c5e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5c5e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /termStore/sets/{setId}
```

## <a name="request-headers"></a><span data-ttu-id="f5c5e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5c5e-118">Request headers</span></span>
|<span data-ttu-id="f5c5e-119">名称</span><span class="sxs-lookup"><span data-stu-id="f5c5e-119">Name</span></span>|<span data-ttu-id="f5c5e-120">说明</span><span class="sxs-lookup"><span data-stu-id="f5c5e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f5c5e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5c5e-121">Authorization</span></span>|<span data-ttu-id="f5c5e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f5c5e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f5c5e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5c5e-124">Content-Type</span></span>|<span data-ttu-id="f5c5e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f5c5e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5c5e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5c5e-127">Request body</span></span>
<span data-ttu-id="f5c5e-128">在请求正文中，提供 set 对象的 JSON [表示](../resources/termstore-set.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="f5c5e-128">In the request body, supply a JSON representation of the [set](../resources/termstore-set.md) object.</span></span>

<span data-ttu-id="f5c5e-129">下表显示了可编辑集 [的属性](../resources/termstore-set.md)。</span><span class="sxs-lookup"><span data-stu-id="f5c5e-129">The following table shows the properties that can be edited for the [set](../resources/termstore-set.md).</span></span>

|<span data-ttu-id="f5c5e-130">属性</span><span class="sxs-lookup"><span data-stu-id="f5c5e-130">Property</span></span>|<span data-ttu-id="f5c5e-131">类型</span><span class="sxs-lookup"><span data-stu-id="f5c5e-131">Type</span></span>|<span data-ttu-id="f5c5e-132">Description</span><span class="sxs-lookup"><span data-stu-id="f5c5e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5c5e-133">localizedNames</span><span class="sxs-lookup"><span data-stu-id="f5c5e-133">localizedNames</span></span>|<span data-ttu-id="f5c5e-134">[microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5c5e-134">[microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md) collection</span></span>|<span data-ttu-id="f5c5e-135">集合的名称</span><span class="sxs-lookup"><span data-stu-id="f5c5e-135">Name of the set</span></span>|
|<span data-ttu-id="f5c5e-136">说明</span><span class="sxs-lookup"><span data-stu-id="f5c5e-136">description</span></span>|<span data-ttu-id="f5c5e-137">String</span><span class="sxs-lookup"><span data-stu-id="f5c5e-137">String</span></span>|<span data-ttu-id="f5c5e-138">集的说明</span><span class="sxs-lookup"><span data-stu-id="f5c5e-138">Description of the set</span></span>|
|<span data-ttu-id="f5c5e-139">properties</span><span class="sxs-lookup"><span data-stu-id="f5c5e-139">properties</span></span>|<span data-ttu-id="f5c5e-140">[microsoft.graph.keyValue](../resources/keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5c5e-140">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="f5c5e-141">集合的属性</span><span class="sxs-lookup"><span data-stu-id="f5c5e-141">properties of a set</span></span>|



## <a name="response"></a><span data-ttu-id="f5c5e-142">响应</span><span class="sxs-lookup"><span data-stu-id="f5c5e-142">Response</span></span>

<span data-ttu-id="f5c5e-143">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和更新的 [set](../resources/termstore-set.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5c5e-143">If successful, this method returns a `200 OK` response code and an updated [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5c5e-144">示例</span><span class="sxs-lookup"><span data-stu-id="f5c5e-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5c5e-145">请求</span><span class="sxs-lookup"><span data-stu-id="f5c5e-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f5c5e-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5c5e-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_set"
} -->

``` http
PATCH https://graph.microsoft.com/beta/termStore/sets/{setId}
Content-Type: application/json
Content-length: 288

{
  "description": "mySet"
}
```
# <a name="c"></a>[<span data-ttu-id="f5c5e-147">C#</span><span class="sxs-lookup"><span data-stu-id="f5c5e-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5c5e-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5c5e-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5c5e-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5c5e-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5c5e-150">Java</span><span class="sxs-lookup"><span data-stu-id="f5c5e-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-set-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f5c5e-151">响应</span><span class="sxs-lookup"><span data-stu-id="f5c5e-151">Response</span></span>

<span data-ttu-id="f5c5e-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f5c5e-152">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.set"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "3607e9f9-e9f9-3607-f9e9-0736f9e90736",
  "description": "mySet",    
  "localizedNames" : [
    {
      "languageTag" : "en-US",
      "name" : "Department"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Update termSet",
  "suppressions": [
  ]
}
-->



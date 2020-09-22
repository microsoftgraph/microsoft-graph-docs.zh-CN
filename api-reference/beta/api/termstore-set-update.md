---
title: 更新集
description: 更新 set 对象的属性。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 3ace6599bab823911dcd5704b7424e198daa4e30
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064582"
---
# <a name="update-set"></a><span data-ttu-id="83775-103">更新集</span><span class="sxs-lookup"><span data-stu-id="83775-103">Update set</span></span>
<span data-ttu-id="83775-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="83775-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83775-105">更新 [set](../resources/termstore-set.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="83775-105">Update the properties of a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="83775-106">权限</span><span class="sxs-lookup"><span data-stu-id="83775-106">Permissions</span></span>
<span data-ttu-id="83775-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83775-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83775-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="83775-109">Permission type</span></span>|<span data-ttu-id="83775-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="83775-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83775-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83775-111">Delegated (work or school account)</span></span> |<span data-ttu-id="83775-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83775-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="83775-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83775-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83775-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="83775-114">Not supported.</span></span>    |
|<span data-ttu-id="83775-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="83775-115">Application</span></span> | <span data-ttu-id="83775-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="83775-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="83775-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83775-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /termStore/sets/{setId}
```

## <a name="request-headers"></a><span data-ttu-id="83775-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="83775-118">Request headers</span></span>
|<span data-ttu-id="83775-119">名称</span><span class="sxs-lookup"><span data-stu-id="83775-119">Name</span></span>|<span data-ttu-id="83775-120">说明</span><span class="sxs-lookup"><span data-stu-id="83775-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="83775-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="83775-121">Authorization</span></span>|<span data-ttu-id="83775-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83775-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="83775-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83775-124">Content-Type</span></span>|<span data-ttu-id="83775-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="83775-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="83775-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="83775-127">Request body</span></span>
<span data-ttu-id="83775-128">在请求正文中，提供 [set](../resources/termstore-set.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83775-128">In the request body, supply a JSON representation of the [set](../resources/termstore-set.md) object.</span></span>

<span data-ttu-id="83775-129">下表显示了可以为该 [集](../resources/termstore-set.md)编辑的属性。</span><span class="sxs-lookup"><span data-stu-id="83775-129">The following table shows the properties that can be edited for the [set](../resources/termstore-set.md).</span></span>

|<span data-ttu-id="83775-130">属性</span><span class="sxs-lookup"><span data-stu-id="83775-130">Property</span></span>|<span data-ttu-id="83775-131">类型</span><span class="sxs-lookup"><span data-stu-id="83775-131">Type</span></span>|<span data-ttu-id="83775-132">说明</span><span class="sxs-lookup"><span data-stu-id="83775-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83775-133">localizedNames</span><span class="sxs-lookup"><span data-stu-id="83775-133">localizedNames</span></span>|<span data-ttu-id="83775-134">[termStore](../resources/termstore-localizedname.md) 集合的 localizedName</span><span class="sxs-lookup"><span data-stu-id="83775-134">[microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md) collection</span></span>|<span data-ttu-id="83775-135">集的名称</span><span class="sxs-lookup"><span data-stu-id="83775-135">Name of the set</span></span>|
|<span data-ttu-id="83775-136">说明</span><span class="sxs-lookup"><span data-stu-id="83775-136">description</span></span>|<span data-ttu-id="83775-137">String</span><span class="sxs-lookup"><span data-stu-id="83775-137">String</span></span>|<span data-ttu-id="83775-138">集的说明</span><span class="sxs-lookup"><span data-stu-id="83775-138">Description of the set</span></span>|
|<span data-ttu-id="83775-139">properties</span><span class="sxs-lookup"><span data-stu-id="83775-139">properties</span></span>|<span data-ttu-id="83775-140">[键值](../resources/keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83775-140">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="83775-141">集的属性</span><span class="sxs-lookup"><span data-stu-id="83775-141">properties of a set</span></span>|



## <a name="response"></a><span data-ttu-id="83775-142">响应</span><span class="sxs-lookup"><span data-stu-id="83775-142">Response</span></span>

<span data-ttu-id="83775-143">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [set](../resources/termstore-set.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83775-143">If successful, this method returns a `200 OK` response code and an updated [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83775-144">示例</span><span class="sxs-lookup"><span data-stu-id="83775-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="83775-145">请求</span><span class="sxs-lookup"><span data-stu-id="83775-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="83775-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="83775-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="83775-147">C#</span><span class="sxs-lookup"><span data-stu-id="83775-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83775-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83775-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83775-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83775-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="83775-150">响应</span><span class="sxs-lookup"><span data-stu-id="83775-150">Response</span></span>

<span data-ttu-id="83775-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="83775-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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



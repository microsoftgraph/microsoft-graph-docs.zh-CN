---
author: JeremyKelley
ms.author: jeremyke
title: 更新捆绑包
description: 更新 Driveitem 的捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 111dbfed3fed6af28c57e04c3437a3a6228c2e3e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987721"
---
# <a name="update-bundle"></a><span data-ttu-id="fc83d-103">更新捆绑包</span><span class="sxs-lookup"><span data-stu-id="fc83d-103">Update bundle</span></span>

<span data-ttu-id="fc83d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc83d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc83d-105">按 ID 更新[driveitem][driveItem]的[捆绑][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="fc83d-105">Update the metadata for a [bundle][] of [driveItems][driveItem] by ID.</span></span>
<span data-ttu-id="fc83d-106">您只能更新以下元数据：</span><span class="sxs-lookup"><span data-stu-id="fc83d-106">You can only update the following metadata:</span></span>

* <span data-ttu-id="fc83d-107">捆绑包名称</span><span class="sxs-lookup"><span data-stu-id="fc83d-107">Bundle name</span></span>
* <span data-ttu-id="fc83d-108">如果适用，则为唱片集 `coverImageItemId` () </span><span class="sxs-lookup"><span data-stu-id="fc83d-108">Album `coverImageItemId` (if applicable)</span></span>

<span data-ttu-id="fc83d-109">任何其他更改请求都将被忽略。</span><span class="sxs-lookup"><span data-stu-id="fc83d-109">Any other change requests will be ignored.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc83d-110">权限</span><span class="sxs-lookup"><span data-stu-id="fc83d-110">Permissions</span></span>

<span data-ttu-id="fc83d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc83d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc83d-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc83d-113">Permission type</span></span>      | <span data-ttu-id="fc83d-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc83d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc83d-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc83d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="fc83d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc83d-116">Not supported.</span></span>                             |
|<span data-ttu-id="fc83d-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc83d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc83d-118">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc83d-118">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="fc83d-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc83d-119">Application</span></span>          | <span data-ttu-id="fc83d-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc83d-120">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="fc83d-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc83d-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="fc83d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc83d-122">Request headers</span></span>

| <span data-ttu-id="fc83d-123">名称</span><span class="sxs-lookup"><span data-stu-id="fc83d-123">Name</span></span>          | <span data-ttu-id="fc83d-124">说明</span><span class="sxs-lookup"><span data-stu-id="fc83d-124">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="fc83d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc83d-125">Authorization</span></span> | <span data-ttu-id="fc83d-126">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="fc83d-126">Bearer \{token\}.</span></span> <span data-ttu-id="fc83d-127">必需。</span><span class="sxs-lookup"><span data-stu-id="fc83d-127">Required.</span></span> |
| <span data-ttu-id="fc83d-128">if-match</span><span class="sxs-lookup"><span data-stu-id="fc83d-128">if-match</span></span>      | <span data-ttu-id="fc83d-129">eTag.</span><span class="sxs-lookup"><span data-stu-id="fc83d-129">eTag.</span></span> <span data-ttu-id="fc83d-130">可选。</span><span class="sxs-lookup"><span data-stu-id="fc83d-130">Optional.</span></span> <span data-ttu-id="fc83d-131">如果包含此请求标头，且提供的 eTag 与 buncle 上的当前 eTag 不匹配， `412 Precondition Failed` 则返回响应。</span><span class="sxs-lookup"><span data-stu-id="fc83d-131">If this request header is included and the eTag provided does not match the current eTag on the buncle, a `412 Precondition Failed` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="fc83d-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc83d-132">Request body</span></span>

<span data-ttu-id="fc83d-133">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="fc83d-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="fc83d-134">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="fc83d-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="fc83d-135">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="fc83d-135">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="fc83d-136">响应</span><span class="sxs-lookup"><span data-stu-id="fc83d-136">Response</span></span>

<span data-ttu-id="fc83d-137">如果成功，此方法将返回一个 [driveItem][] 资源，该资源表示响应正文中更新的捆绑包。</span><span class="sxs-lookup"><span data-stu-id="fc83d-137">If successful, this method returns a [driveItem][] resource that represents the updated bundle in the response body.</span></span>

<span data-ttu-id="fc83d-138">阅读 " [错误响应][error-response] " 主题，了解有关如何返回错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fc83d-138">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="fc83d-139">示例</span><span class="sxs-lookup"><span data-stu-id="fc83d-139">Example</span></span>

<span data-ttu-id="fc83d-140">此示例重命名捆绑包。</span><span class="sxs-lookup"><span data-stu-id="fc83d-140">This example renames a bundle.</span></span>

### <a name="request"></a><span data-ttu-id="fc83d-141">请求</span><span class="sxs-lookup"><span data-stu-id="fc83d-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fc83d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc83d-142">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "rename-bundle" } -->

```json
PATCH https://graph.microsoft.com/beta/drive/items/{bundle-id}
Content-Type: application/json

{
  "name": "Shared legal agreements"
}
```
# <a name="c"></a>[<span data-ttu-id="fc83d-143">C#</span><span class="sxs-lookup"><span data-stu-id="fc83d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rename-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc83d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc83d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rename-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc83d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc83d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rename-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fc83d-146">响应</span><span class="sxs-lookup"><span data-stu-id="fc83d-146">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "Shared legal agreements",
  "bundle": {
    "childCount": 3
  }
}
```

<span data-ttu-id="fc83d-147">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fc83d-147">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fc83d-148">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fc83d-148">All the properties will be returned from an actual call.</span></span>


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of a bundle.",
  "keywords": "update,replace,contents,bundle",
  "section": "documentation",
    "tocPath": "Bundles/Update"
} -->



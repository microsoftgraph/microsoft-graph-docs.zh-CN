---
author: JeremyKelley
ms.author: jeremyke
title: 更新捆绑包
description: 更新 Driveitem 的捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: af14454f660761a6e8fc6304d23870d5216540fc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960179"
---
# <a name="update-bundle"></a><span data-ttu-id="5983f-103">更新捆绑包</span><span class="sxs-lookup"><span data-stu-id="5983f-103">Update bundle</span></span>

<span data-ttu-id="5983f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5983f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5983f-105">按 ID 更新[driveitem][driveItem]的[捆绑][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="5983f-105">Update the metadata for a [bundle][] of [driveItems][driveItem] by ID.</span></span>
<span data-ttu-id="5983f-106">您只能更新以下元数据：</span><span class="sxs-lookup"><span data-stu-id="5983f-106">You can only update the following metadata:</span></span>

* <span data-ttu-id="5983f-107">捆绑包名称</span><span class="sxs-lookup"><span data-stu-id="5983f-107">Bundle name</span></span>
* <span data-ttu-id="5983f-108">如果适用，则为唱片集 `coverImageItemId` () </span><span class="sxs-lookup"><span data-stu-id="5983f-108">Album `coverImageItemId` (if applicable)</span></span>

<span data-ttu-id="5983f-109">任何其他更改请求都将被忽略。</span><span class="sxs-lookup"><span data-stu-id="5983f-109">Any other change requests will be ignored.</span></span>

## <a name="permissions"></a><span data-ttu-id="5983f-110">权限</span><span class="sxs-lookup"><span data-stu-id="5983f-110">Permissions</span></span>

<span data-ttu-id="5983f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5983f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5983f-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="5983f-113">Permission type</span></span>      | <span data-ttu-id="5983f-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5983f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5983f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5983f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="5983f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5983f-116">Not supported.</span></span>                             |
|<span data-ttu-id="5983f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5983f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5983f-118">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5983f-118">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="5983f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="5983f-119">Application</span></span>          | <span data-ttu-id="5983f-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="5983f-120">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="5983f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5983f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="5983f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5983f-122">Request headers</span></span>

| <span data-ttu-id="5983f-123">名称</span><span class="sxs-lookup"><span data-stu-id="5983f-123">Name</span></span>          | <span data-ttu-id="5983f-124">说明</span><span class="sxs-lookup"><span data-stu-id="5983f-124">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="5983f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5983f-125">Authorization</span></span> | <span data-ttu-id="5983f-126">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="5983f-126">Bearer \{token\}.</span></span> <span data-ttu-id="5983f-127">必需。</span><span class="sxs-lookup"><span data-stu-id="5983f-127">Required.</span></span> |
| <span data-ttu-id="5983f-128">if-match</span><span class="sxs-lookup"><span data-stu-id="5983f-128">if-match</span></span>      | <span data-ttu-id="5983f-129">eTag.</span><span class="sxs-lookup"><span data-stu-id="5983f-129">eTag.</span></span> <span data-ttu-id="5983f-130">可选。</span><span class="sxs-lookup"><span data-stu-id="5983f-130">Optional.</span></span> <span data-ttu-id="5983f-131">如果包含此请求标头，且提供的 eTag 与 buncle 上的当前 eTag 不匹配， `412 Precondition Failed` 则返回响应。</span><span class="sxs-lookup"><span data-stu-id="5983f-131">If this request header is included and the eTag provided does not match the current eTag on the buncle, a `412 Precondition Failed` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="5983f-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="5983f-132">Request body</span></span>

<span data-ttu-id="5983f-133">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="5983f-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5983f-134">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="5983f-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5983f-135">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5983f-135">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="5983f-136">响应</span><span class="sxs-lookup"><span data-stu-id="5983f-136">Response</span></span>

<span data-ttu-id="5983f-137">如果成功，此方法将返回一个 [driveItem][] 资源，该资源表示响应正文中更新的捆绑包。</span><span class="sxs-lookup"><span data-stu-id="5983f-137">If successful, this method returns a [driveItem][] resource that represents the updated bundle in the response body.</span></span>

<span data-ttu-id="5983f-138">阅读 " [错误响应][error-response] " 主题，了解有关如何返回错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5983f-138">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="5983f-139">示例</span><span class="sxs-lookup"><span data-stu-id="5983f-139">Example</span></span>

<span data-ttu-id="5983f-140">此示例重命名捆绑包。</span><span class="sxs-lookup"><span data-stu-id="5983f-140">This example renames a bundle.</span></span>

### <a name="request"></a><span data-ttu-id="5983f-141">请求</span><span class="sxs-lookup"><span data-stu-id="5983f-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5983f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5983f-142">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "rename-bundle" } -->

```json
PATCH https://graph.microsoft.com/beta/drive/items/{bundle-id}
Content-Type: application/json

{
  "name": "Shared legal agreements"
}
```
# <a name="c"></a>[<span data-ttu-id="5983f-143">C#</span><span class="sxs-lookup"><span data-stu-id="5983f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rename-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5983f-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5983f-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rename-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5983f-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5983f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rename-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5983f-146">Java</span><span class="sxs-lookup"><span data-stu-id="5983f-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rename-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5983f-147">响应</span><span class="sxs-lookup"><span data-stu-id="5983f-147">Response</span></span>

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

<span data-ttu-id="5983f-148">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5983f-148">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5983f-149">所有属性都是从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5983f-149">All the properties will be returned from an actual call.</span></span>


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



---
author: JeremyKelley
title: 更新捆绑包
description: 更新 driveItems 捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 7b6cd4001acd674d265748e24638c2bca5454967
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047775"
---
# <a name="update-bundle"></a><span data-ttu-id="573d9-103">更新捆绑包</span><span class="sxs-lookup"><span data-stu-id="573d9-103">Update bundle</span></span>

<span data-ttu-id="573d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="573d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="573d9-105">按 ID[更新][][driveItems][driveItem 捆绑]包的元数据。</span><span class="sxs-lookup"><span data-stu-id="573d9-105">Update the metadata for a [bundle][] of [driveItems][driveItem] by ID.</span></span>
<span data-ttu-id="573d9-106">只能更新以下元数据：</span><span class="sxs-lookup"><span data-stu-id="573d9-106">You can only update the following metadata:</span></span>

* <span data-ttu-id="573d9-107">捆绑包名称</span><span class="sxs-lookup"><span data-stu-id="573d9-107">Bundle name</span></span>
* <span data-ttu-id="573d9-108">专辑 `coverImageItemId` (（如果适用) </span><span class="sxs-lookup"><span data-stu-id="573d9-108">Album `coverImageItemId` (if applicable)</span></span>

<span data-ttu-id="573d9-109">将忽略任何其他更改请求。</span><span class="sxs-lookup"><span data-stu-id="573d9-109">Any other change requests will be ignored.</span></span>

## <a name="permissions"></a><span data-ttu-id="573d9-110">权限</span><span class="sxs-lookup"><span data-stu-id="573d9-110">Permissions</span></span>

<span data-ttu-id="573d9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="573d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="573d9-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="573d9-113">Permission type</span></span>      | <span data-ttu-id="573d9-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="573d9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="573d9-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="573d9-115">Delegated (work or school account)</span></span> | <span data-ttu-id="573d9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="573d9-116">Not supported.</span></span>                             |
|<span data-ttu-id="573d9-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="573d9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="573d9-118">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="573d9-118">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="573d9-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="573d9-119">Application</span></span>          | <span data-ttu-id="573d9-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="573d9-120">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="573d9-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="573d9-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="573d9-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="573d9-122">Request headers</span></span>

| <span data-ttu-id="573d9-123">名称</span><span class="sxs-lookup"><span data-stu-id="573d9-123">Name</span></span>          | <span data-ttu-id="573d9-124">说明</span><span class="sxs-lookup"><span data-stu-id="573d9-124">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="573d9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="573d9-125">Authorization</span></span> | <span data-ttu-id="573d9-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="573d9-p103">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="573d9-128">if-match</span><span class="sxs-lookup"><span data-stu-id="573d9-128">if-match</span></span>      | <span data-ttu-id="573d9-129">eTag。</span><span class="sxs-lookup"><span data-stu-id="573d9-129">eTag.</span></span> <span data-ttu-id="573d9-130">可选。</span><span class="sxs-lookup"><span data-stu-id="573d9-130">Optional.</span></span> <span data-ttu-id="573d9-131">如果包含此请求标头，并且提供的 eTag 与 buncle 上的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应。</span><span class="sxs-lookup"><span data-stu-id="573d9-131">If this request header is included and the eTag provided does not match the current eTag on the buncle, a `412 Precondition Failed` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="573d9-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="573d9-132">Request body</span></span>

<span data-ttu-id="573d9-133">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="573d9-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="573d9-134">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="573d9-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="573d9-135">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="573d9-135">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="573d9-136">响应</span><span class="sxs-lookup"><span data-stu-id="573d9-136">Response</span></span>

<span data-ttu-id="573d9-137">如果成功，此方法在响应正文中返回表示更新捆绑包的 [driveItem][] 资源。</span><span class="sxs-lookup"><span data-stu-id="573d9-137">If successful, this method returns a [driveItem][] resource that represents the updated bundle in the response body.</span></span>

<span data-ttu-id="573d9-138">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="573d9-138">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="573d9-139">示例</span><span class="sxs-lookup"><span data-stu-id="573d9-139">Example</span></span>

<span data-ttu-id="573d9-140">此示例重命名捆绑包。</span><span class="sxs-lookup"><span data-stu-id="573d9-140">This example renames a bundle.</span></span>

### <a name="request"></a><span data-ttu-id="573d9-141">请求</span><span class="sxs-lookup"><span data-stu-id="573d9-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="573d9-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="573d9-142">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "rename-bundle" } -->

```http
PATCH https://graph.microsoft.com/beta/drive/items/{bundle-id}
Content-Type: application/json

{
  "name": "Shared legal agreements"
}
```
# <a name="c"></a>[<span data-ttu-id="573d9-143">C#</span><span class="sxs-lookup"><span data-stu-id="573d9-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rename-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="573d9-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="573d9-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rename-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="573d9-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="573d9-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rename-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="573d9-146">Java</span><span class="sxs-lookup"><span data-stu-id="573d9-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rename-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="573d9-147">响应</span><span class="sxs-lookup"><span data-stu-id="573d9-147">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
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

<span data-ttu-id="573d9-148">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="573d9-148">The response object shown here might be shortened for readability.</span></span>


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of a bundle.",
  "keywords": "update,replace,contents,bundle",
  "section": "documentation",
    "tocPath&quot;: &quot;Bundles/Update"
} -->



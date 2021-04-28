---
title: driveItem： restore
description: 还原已删除且当前位于回收站中的 driveItem。
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: apiPageType
ms.openlocfilehash: 391788bccc09876a1bed78da932dd574f1e23cfb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054047"
---
# <a name="driveitem-restore"></a><span data-ttu-id="2ce5e-103">driveItem： restore</span><span class="sxs-lookup"><span data-stu-id="2ce5e-103">driveItem: restore</span></span>

<span data-ttu-id="2ce5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ce5e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2ce5e-105">还原已删除且当前位于回收站中的[driveItem。](../resources/driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="2ce5e-105">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="2ce5e-106">**注意**：此功能当前仅适用于个人OneDrive。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-106">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ce5e-107">权限</span><span class="sxs-lookup"><span data-stu-id="2ce5e-107">Permissions</span></span>

<span data-ttu-id="2ce5e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ce5e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ce5e-110">Permission type</span></span>                        | <span data-ttu-id="2ce5e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ce5e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2ce5e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ce5e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ce5e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-113">Not supported.</span></span> |
| <span data-ttu-id="2ce5e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ce5e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ce5e-115">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ce5e-115">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="2ce5e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ce5e-116">Application</span></span>                            | <span data-ttu-id="2ce5e-117">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ce5e-117">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ce5e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ce5e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="2ce5e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ce5e-119">Request headers</span></span>

| <span data-ttu-id="2ce5e-120">名称</span><span class="sxs-lookup"><span data-stu-id="2ce5e-120">Name</span></span>          | <span data-ttu-id="2ce5e-121">说明</span><span class="sxs-lookup"><span data-stu-id="2ce5e-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2ce5e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ce5e-122">Authorization</span></span> | <span data-ttu-id="2ce5e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ce5e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ce5e-125">Request body</span></span>

<span data-ttu-id="2ce5e-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2ce5e-127">参数</span><span class="sxs-lookup"><span data-stu-id="2ce5e-127">Parameter</span></span>     | <span data-ttu-id="2ce5e-128">类型</span><span class="sxs-lookup"><span data-stu-id="2ce5e-128">Type</span></span>                                         | <span data-ttu-id="2ce5e-129">说明</span><span class="sxs-lookup"><span data-stu-id="2ce5e-129">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="2ce5e-130">parentReference</span><span class="sxs-lookup"><span data-stu-id="2ce5e-130">parentReference</span></span>|[<span data-ttu-id="2ce5e-131">ItemReference</span><span class="sxs-lookup"><span data-stu-id="2ce5e-131">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="2ce5e-132">可选。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-132">Optional.</span></span> <span data-ttu-id="2ce5e-133">对已删除项目将还原到的父项的引用。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-133">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="2ce5e-134">name</span><span class="sxs-lookup"><span data-stu-id="2ce5e-134">name</span></span>           |<span data-ttu-id="2ce5e-135">String</span><span class="sxs-lookup"><span data-stu-id="2ce5e-135">String</span></span>                                        | <span data-ttu-id="2ce5e-136">可选。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-136">Optional.</span></span> <span data-ttu-id="2ce5e-137">已还原项目的新名称。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-137">The new name for the restored item.</span></span> <span data-ttu-id="2ce5e-138">如果未提供新名称，将同一名称用作原始名称。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-138">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="2ce5e-139">响应</span><span class="sxs-lookup"><span data-stu-id="2ce5e-139">Response</span></span>

<span data-ttu-id="2ce5e-140">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` 已还原的 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-140">If successful, this method returns a `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ce5e-141">示例</span><span class="sxs-lookup"><span data-stu-id="2ce5e-141">Examples</span></span>

<span data-ttu-id="2ce5e-142">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-142">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2ce5e-143">请求</span><span class="sxs-lookup"><span data-stu-id="2ce5e-143">Request</span></span>

<span data-ttu-id="2ce5e-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ce5e-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ce5e-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "restore-item",
  "scopes": "files.readwrite",
  "target": "action"
}-->

```http
POST https://graph.microsoft.com/beta/me/drive/items/{item-id}/restore
Content-type: application/json

{
  "parentReference": {
    "id": "String",
  },
  "name": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="2ce5e-146">C#</span><span class="sxs-lookup"><span data-stu-id="2ce5e-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ce5e-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ce5e-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ce5e-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ce5e-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ce5e-149">Java</span><span class="sxs-lookup"><span data-stu-id="2ce5e-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ce5e-150">响应</span><span class="sxs-lookup"><span data-stu-id="2ce5e-150">Response</span></span>

<span data-ttu-id="2ce5e-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-151">The following is an example of the response.</span></span>

> <span data-ttu-id="2ce5e-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2ce5e-152">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1312abc!1231",
  "name": "new-restored-item-name.txt",
  "size": 19121,
  "lastModifiedDateTime": "2017-12-12T10:40:59Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Restore a DriveItem.",
  "keywords": "retore,item,driveitem",
  "section": "documentation",
  "tocPath": "Items/Restore"
}-->


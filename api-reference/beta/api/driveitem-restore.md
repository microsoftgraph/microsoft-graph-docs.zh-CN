---
title: driveItem： restore
description: 还原已删除且当前在回收站中的 driveItem。
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
ms.date: 08/06/2019
doc_type: apiPageType
ms.openlocfilehash: fc2d7e73fb3c3ad781025e84166845dc84c3bdde
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981889"
---
# <a name="driveitem-restore"></a><span data-ttu-id="49caa-103">driveItem： restore</span><span class="sxs-lookup"><span data-stu-id="49caa-103">driveItem: restore</span></span>

<span data-ttu-id="49caa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49caa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49caa-105">还原已删除且当前在回收站中的 [driveItem](../resources/driveitem.md) 。</span><span class="sxs-lookup"><span data-stu-id="49caa-105">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="49caa-106">**注意**：此功能目前仅适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="49caa-106">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="49caa-107">权限</span><span class="sxs-lookup"><span data-stu-id="49caa-107">Permissions</span></span>

<span data-ttu-id="49caa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49caa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49caa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="49caa-110">Permission type</span></span>                        | <span data-ttu-id="49caa-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49caa-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="49caa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49caa-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="49caa-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="49caa-113">Not supported.</span></span> |
| <span data-ttu-id="49caa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49caa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49caa-115">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49caa-115">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="49caa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="49caa-116">Application</span></span>                            | <span data-ttu-id="49caa-117">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49caa-117">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49caa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49caa-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="49caa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="49caa-119">Request headers</span></span>

| <span data-ttu-id="49caa-120">名称</span><span class="sxs-lookup"><span data-stu-id="49caa-120">Name</span></span>          | <span data-ttu-id="49caa-121">说明</span><span class="sxs-lookup"><span data-stu-id="49caa-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="49caa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="49caa-122">Authorization</span></span> | <span data-ttu-id="49caa-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="49caa-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="49caa-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="49caa-124">Request body</span></span>

<span data-ttu-id="49caa-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="49caa-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="49caa-126">参数</span><span class="sxs-lookup"><span data-stu-id="49caa-126">Parameter</span></span>     | <span data-ttu-id="49caa-127">类型</span><span class="sxs-lookup"><span data-stu-id="49caa-127">Type</span></span>                                         | <span data-ttu-id="49caa-128">说明</span><span class="sxs-lookup"><span data-stu-id="49caa-128">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="49caa-129">parentReference</span><span class="sxs-lookup"><span data-stu-id="49caa-129">parentReference</span></span>|[<span data-ttu-id="49caa-130">ItemReference</span><span class="sxs-lookup"><span data-stu-id="49caa-130">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="49caa-131">可选。</span><span class="sxs-lookup"><span data-stu-id="49caa-131">Optional.</span></span> <span data-ttu-id="49caa-132">对父项的引用，已删除的项将还原到该父项。</span><span class="sxs-lookup"><span data-stu-id="49caa-132">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="49caa-133">name</span><span class="sxs-lookup"><span data-stu-id="49caa-133">name</span></span>           |<span data-ttu-id="49caa-134">String</span><span class="sxs-lookup"><span data-stu-id="49caa-134">String</span></span>                                        | <span data-ttu-id="49caa-135">可选。</span><span class="sxs-lookup"><span data-stu-id="49caa-135">Optional.</span></span> <span data-ttu-id="49caa-136">已还原的项的新名称。</span><span class="sxs-lookup"><span data-stu-id="49caa-136">The new name for the restored item.</span></span> <span data-ttu-id="49caa-137">如果未提供新名称，将同一名称用作原始名称。</span><span class="sxs-lookup"><span data-stu-id="49caa-137">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="49caa-138">响应</span><span class="sxs-lookup"><span data-stu-id="49caa-138">Response</span></span>

<span data-ttu-id="49caa-139">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和还原的 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="49caa-139">If successful, this method returns `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49caa-140">示例</span><span class="sxs-lookup"><span data-stu-id="49caa-140">Examples</span></span>

<span data-ttu-id="49caa-141">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="49caa-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="49caa-142">请求</span><span class="sxs-lookup"><span data-stu-id="49caa-142">Request</span></span>

<span data-ttu-id="49caa-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="49caa-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49caa-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="49caa-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="49caa-145">C#</span><span class="sxs-lookup"><span data-stu-id="49caa-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49caa-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49caa-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49caa-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49caa-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="49caa-148">响应</span><span class="sxs-lookup"><span data-stu-id="49caa-148">Response</span></span>

<span data-ttu-id="49caa-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="49caa-149">The following is an example of the response.</span></span>

> <span data-ttu-id="49caa-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="49caa-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



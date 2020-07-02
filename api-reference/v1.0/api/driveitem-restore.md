---
title: driveItem： restore
description: 还原已删除且当前在回收站中的 driveItem。
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: apiPageType
ms.openlocfilehash: 86c658ad853a11f3ff7a52a6efeb7b2cc1bdb6c2
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007093"
---
# <a name="driveitem-restore"></a><span data-ttu-id="48f14-103">driveItem： restore</span><span class="sxs-lookup"><span data-stu-id="48f14-103">driveItem: restore</span></span>

<span data-ttu-id="48f14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48f14-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48f14-105">还原已删除且当前在回收站中的[driveItem](../resources/driveitem.md) 。</span><span class="sxs-lookup"><span data-stu-id="48f14-105">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="48f14-106">**注意**：此功能目前仅适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="48f14-106">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="48f14-107">权限</span><span class="sxs-lookup"><span data-stu-id="48f14-107">Permissions</span></span>

<span data-ttu-id="48f14-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="48f14-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="48f14-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48f14-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48f14-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="48f14-110">Permission type</span></span>                        | <span data-ttu-id="48f14-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="48f14-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="48f14-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48f14-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="48f14-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="48f14-113">Not supported.</span></span> |
| <span data-ttu-id="48f14-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48f14-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48f14-115">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f14-115">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="48f14-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="48f14-116">Application</span></span>                            | <span data-ttu-id="48f14-117">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f14-117">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48f14-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48f14-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="48f14-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="48f14-119">Request headers</span></span>

| <span data-ttu-id="48f14-120">名称</span><span class="sxs-lookup"><span data-stu-id="48f14-120">Name</span></span>          | <span data-ttu-id="48f14-121">说明</span><span class="sxs-lookup"><span data-stu-id="48f14-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="48f14-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="48f14-122">Authorization</span></span> | <span data-ttu-id="48f14-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="48f14-123">Bearer {token}.</span></span> <span data-ttu-id="48f14-124">Required.</span><span class="sxs-lookup"><span data-stu-id="48f14-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48f14-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="48f14-125">Request body</span></span>

<span data-ttu-id="48f14-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="48f14-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="48f14-127">参数</span><span class="sxs-lookup"><span data-stu-id="48f14-127">Parameter</span></span>     | <span data-ttu-id="48f14-128">类型</span><span class="sxs-lookup"><span data-stu-id="48f14-128">Type</span></span>                                         | <span data-ttu-id="48f14-129">说明</span><span class="sxs-lookup"><span data-stu-id="48f14-129">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="48f14-130">parentReference</span><span class="sxs-lookup"><span data-stu-id="48f14-130">parentReference</span></span>|[<span data-ttu-id="48f14-131">ItemReference</span><span class="sxs-lookup"><span data-stu-id="48f14-131">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="48f14-132">可选。</span><span class="sxs-lookup"><span data-stu-id="48f14-132">Optional.</span></span> <span data-ttu-id="48f14-133">对父项的引用，已删除的项将还原到该父项。</span><span class="sxs-lookup"><span data-stu-id="48f14-133">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="48f14-134">name</span><span class="sxs-lookup"><span data-stu-id="48f14-134">name</span></span>           |<span data-ttu-id="48f14-135">String</span><span class="sxs-lookup"><span data-stu-id="48f14-135">String</span></span>                                        | <span data-ttu-id="48f14-136">可选。</span><span class="sxs-lookup"><span data-stu-id="48f14-136">Optional.</span></span> <span data-ttu-id="48f14-137">已还原的项的新名称。</span><span class="sxs-lookup"><span data-stu-id="48f14-137">The new name for the restored item.</span></span> <span data-ttu-id="48f14-138">如果未提供新名称，将同一名称用作原始名称。</span><span class="sxs-lookup"><span data-stu-id="48f14-138">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="48f14-139">响应</span><span class="sxs-lookup"><span data-stu-id="48f14-139">Response</span></span>

<span data-ttu-id="48f14-140">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和还原的[driveItem](../resources/driveitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="48f14-140">If successful, this method returns a `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48f14-141">示例</span><span class="sxs-lookup"><span data-stu-id="48f14-141">Examples</span></span>

<span data-ttu-id="48f14-142">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="48f14-142">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="48f14-143">请求</span><span class="sxs-lookup"><span data-stu-id="48f14-143">Request</span></span>

<span data-ttu-id="48f14-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="48f14-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="48f14-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="48f14-145">HTTP</span></span>](#tab/http)

# <a name="http"></a>[<span data-ttu-id="48f14-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="48f14-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="48f14-147">C#</span><span class="sxs-lookup"><span data-stu-id="48f14-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48f14-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48f14-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48f14-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48f14-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="48f14-150">响应</span><span class="sxs-lookup"><span data-stu-id="48f14-150">Response</span></span>

<span data-ttu-id="48f14-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="48f14-151">The following is an example of the response.</span></span>

> <span data-ttu-id="48f14-152">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="48f14-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="48f14-153">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="48f14-153">All the properties will be returned from an actual call.</span></span>

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

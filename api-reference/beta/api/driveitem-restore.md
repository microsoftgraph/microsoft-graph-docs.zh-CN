---
title: driveItem： restore
description: 还原已删除且当前在回收站中的 driveItem。
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
ms.date: 08/06/2019
doc_type: apiPageType
ms.openlocfilehash: f105ab748e6fff69f1138e4318ac66597a721391
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356294"
---
# <a name="driveitem-restore"></a><span data-ttu-id="d45d3-103">driveItem： restore</span><span class="sxs-lookup"><span data-stu-id="d45d3-103">driveItem: restore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d45d3-104">还原已删除且当前在回收站中的[driveItem](../resources/driveitem.md) 。</span><span class="sxs-lookup"><span data-stu-id="d45d3-104">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="d45d3-105">**注意**：此功能目前仅适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="d45d3-105">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="d45d3-106">权限</span><span class="sxs-lookup"><span data-stu-id="d45d3-106">Permissions</span></span>

<span data-ttu-id="d45d3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d45d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d45d3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d45d3-109">Permission type</span></span>                        | <span data-ttu-id="d45d3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d45d3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d45d3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d45d3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d45d3-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="d45d3-112">Not supported.</span></span> |
| <span data-ttu-id="d45d3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d45d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d45d3-114">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d45d3-114">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="d45d3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d45d3-115">Application</span></span>                            | <span data-ttu-id="d45d3-116">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d45d3-116">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d45d3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d45d3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="d45d3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d45d3-118">Request headers</span></span>

| <span data-ttu-id="d45d3-119">名称</span><span class="sxs-lookup"><span data-stu-id="d45d3-119">Name</span></span>          | <span data-ttu-id="d45d3-120">说明</span><span class="sxs-lookup"><span data-stu-id="d45d3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d45d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d45d3-121">Authorization</span></span> | <span data-ttu-id="d45d3-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d45d3-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d45d3-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d45d3-123">Request body</span></span>

<span data-ttu-id="d45d3-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d45d3-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d45d3-125">参数</span><span class="sxs-lookup"><span data-stu-id="d45d3-125">Parameter</span></span>     | <span data-ttu-id="d45d3-126">类型</span><span class="sxs-lookup"><span data-stu-id="d45d3-126">Type</span></span>                                         | <span data-ttu-id="d45d3-127">说明</span><span class="sxs-lookup"><span data-stu-id="d45d3-127">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="d45d3-128">parentReference</span><span class="sxs-lookup"><span data-stu-id="d45d3-128">parentReference</span></span>|[<span data-ttu-id="d45d3-129">ItemReference</span><span class="sxs-lookup"><span data-stu-id="d45d3-129">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="d45d3-130">可选。</span><span class="sxs-lookup"><span data-stu-id="d45d3-130">Optional.</span></span> <span data-ttu-id="d45d3-131">对父项的引用，已删除的项将还原到该父项。</span><span class="sxs-lookup"><span data-stu-id="d45d3-131">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="d45d3-132">name</span><span class="sxs-lookup"><span data-stu-id="d45d3-132">name</span></span>           |<span data-ttu-id="d45d3-133">String</span><span class="sxs-lookup"><span data-stu-id="d45d3-133">String</span></span>                                        | <span data-ttu-id="d45d3-134">可选。</span><span class="sxs-lookup"><span data-stu-id="d45d3-134">Optional.</span></span> <span data-ttu-id="d45d3-135">已还原的项的新名称。</span><span class="sxs-lookup"><span data-stu-id="d45d3-135">The new name for the restored item.</span></span> <span data-ttu-id="d45d3-136">如果未提供新名称，将同一名称用作原始名称。</span><span class="sxs-lookup"><span data-stu-id="d45d3-136">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="d45d3-137">响应</span><span class="sxs-lookup"><span data-stu-id="d45d3-137">Response</span></span>

<span data-ttu-id="d45d3-138">如果成功，此方法在`200 OK`响应正文中返回响应代码和还原的[driveItem](../resources/driveitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d45d3-138">If successful, this method returns `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d45d3-139">示例</span><span class="sxs-lookup"><span data-stu-id="d45d3-139">Examples</span></span>

<span data-ttu-id="d45d3-140">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d45d3-140">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d45d3-141">请求</span><span class="sxs-lookup"><span data-stu-id="d45d3-141">Request</span></span>

<span data-ttu-id="d45d3-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d45d3-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d45d3-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d45d3-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d45d3-144">C#</span><span class="sxs-lookup"><span data-stu-id="d45d3-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d45d3-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d45d3-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d45d3-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d45d3-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d45d3-147">响应</span><span class="sxs-lookup"><span data-stu-id="d45d3-147">Response</span></span>

<span data-ttu-id="d45d3-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d45d3-148">The following is an example of the response.</span></span>

> <span data-ttu-id="d45d3-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d45d3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

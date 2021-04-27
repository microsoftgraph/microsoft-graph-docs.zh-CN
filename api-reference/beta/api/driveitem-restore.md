---
title: driveItem： restore
description: 还原已删除且当前位于回收站中的 driveItem。
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
ms.date: 08/06/2019
doc_type: apiPageType
ms.openlocfilehash: fc1d9e1dc44af3ccbca132d8d54f1413e029f614
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046263"
---
# <a name="driveitem-restore"></a><span data-ttu-id="585cf-103">driveItem： restore</span><span class="sxs-lookup"><span data-stu-id="585cf-103">driveItem: restore</span></span>

<span data-ttu-id="585cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="585cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="585cf-105">还原已删除且当前位于回收站中的[driveItem。](../resources/driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="585cf-105">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="585cf-106">**注意**：此功能当前仅适用于个人OneDrive。</span><span class="sxs-lookup"><span data-stu-id="585cf-106">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="585cf-107">权限</span><span class="sxs-lookup"><span data-stu-id="585cf-107">Permissions</span></span>

<span data-ttu-id="585cf-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="585cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="585cf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="585cf-110">Permission type</span></span>                        | <span data-ttu-id="585cf-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="585cf-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="585cf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="585cf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="585cf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="585cf-113">Not supported.</span></span> |
| <span data-ttu-id="585cf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="585cf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="585cf-115">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="585cf-115">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="585cf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="585cf-116">Application</span></span>                            | <span data-ttu-id="585cf-117">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="585cf-117">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="585cf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="585cf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="585cf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="585cf-119">Request headers</span></span>

| <span data-ttu-id="585cf-120">名称</span><span class="sxs-lookup"><span data-stu-id="585cf-120">Name</span></span>          | <span data-ttu-id="585cf-121">说明</span><span class="sxs-lookup"><span data-stu-id="585cf-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="585cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="585cf-122">Authorization</span></span> | <span data-ttu-id="585cf-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="585cf-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="585cf-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="585cf-124">Request body</span></span>

<span data-ttu-id="585cf-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="585cf-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="585cf-126">参数</span><span class="sxs-lookup"><span data-stu-id="585cf-126">Parameter</span></span>     | <span data-ttu-id="585cf-127">类型</span><span class="sxs-lookup"><span data-stu-id="585cf-127">Type</span></span>                                         | <span data-ttu-id="585cf-128">说明</span><span class="sxs-lookup"><span data-stu-id="585cf-128">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="585cf-129">parentReference</span><span class="sxs-lookup"><span data-stu-id="585cf-129">parentReference</span></span>|[<span data-ttu-id="585cf-130">ItemReference</span><span class="sxs-lookup"><span data-stu-id="585cf-130">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="585cf-131">可选。</span><span class="sxs-lookup"><span data-stu-id="585cf-131">Optional.</span></span> <span data-ttu-id="585cf-132">对已删除项目将还原到的父项的引用。</span><span class="sxs-lookup"><span data-stu-id="585cf-132">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="585cf-133">name</span><span class="sxs-lookup"><span data-stu-id="585cf-133">name</span></span>           |<span data-ttu-id="585cf-134">String</span><span class="sxs-lookup"><span data-stu-id="585cf-134">String</span></span>                                        | <span data-ttu-id="585cf-135">可选。</span><span class="sxs-lookup"><span data-stu-id="585cf-135">Optional.</span></span> <span data-ttu-id="585cf-136">已还原项目的新名称。</span><span class="sxs-lookup"><span data-stu-id="585cf-136">The new name for the restored item.</span></span> <span data-ttu-id="585cf-137">如果未提供新名称，将同一名称用作原始名称。</span><span class="sxs-lookup"><span data-stu-id="585cf-137">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="585cf-138">响应</span><span class="sxs-lookup"><span data-stu-id="585cf-138">Response</span></span>

<span data-ttu-id="585cf-139">如果成功，此方法在 `200 OK` 响应正文中返回 响应代码和已还原的 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="585cf-139">If successful, this method returns `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="585cf-140">示例</span><span class="sxs-lookup"><span data-stu-id="585cf-140">Examples</span></span>

<span data-ttu-id="585cf-141">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="585cf-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="585cf-142">请求</span><span class="sxs-lookup"><span data-stu-id="585cf-142">Request</span></span>

<span data-ttu-id="585cf-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="585cf-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="585cf-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="585cf-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="585cf-145">C#</span><span class="sxs-lookup"><span data-stu-id="585cf-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="585cf-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="585cf-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="585cf-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="585cf-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="585cf-148">Java</span><span class="sxs-lookup"><span data-stu-id="585cf-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="585cf-149">响应</span><span class="sxs-lookup"><span data-stu-id="585cf-149">Response</span></span>

<span data-ttu-id="585cf-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="585cf-150">The following is an example of the response.</span></span>

> <span data-ttu-id="585cf-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="585cf-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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



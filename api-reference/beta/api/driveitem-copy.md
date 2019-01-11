---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 复制文件或文件夹
localization_priority: Normal
ms.openlocfilehash: 8289bd3c15575e1469fe18baf45c6c2f937ed2dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879441"
---
# <a name="copy-a-driveitem"></a><span data-ttu-id="a4e4d-102">复制 DriveItem</span><span class="sxs-lookup"><span data-stu-id="a4e4d-102">Copy a DriveItem</span></span>

> <span data-ttu-id="a4e4d-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a4e4d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4e4d-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a4e4d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4e4d-105">以异步方式在新父项下或使用新名称创建一个 [driveItem][item-resource] 副本（包括任何子项）。</span><span class="sxs-lookup"><span data-stu-id="a4e4d-105">Asynchronously creates a copy of an [driveItem][item-resource] (including any children), under a new parent item or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4e4d-106">权限</span><span class="sxs-lookup"><span data-stu-id="a4e4d-106">Permissions</span></span>

<span data-ttu-id="a4e4d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4e4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4e4d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4e4d-109">Permission type</span></span>      | <span data-ttu-id="a4e4d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4e4d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4e4d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4e4d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a4e4d-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4e4d-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a4e4d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4e4d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4e4d-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4e4d-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a4e4d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4e4d-115">Application</span></span> | <span data-ttu-id="a4e4d-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4e4d-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4e4d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4e4d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a><span data-ttu-id="a4e4d-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4e4d-118">Request body</span></span>

<span data-ttu-id="a4e4d-119">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a4e4d-119">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="a4e4d-120">名称</span><span class="sxs-lookup"><span data-stu-id="a4e4d-120">Name</span></span>            | <span data-ttu-id="a4e4d-121">值</span><span class="sxs-lookup"><span data-stu-id="a4e4d-121">Value</span></span>                                          | <span data-ttu-id="a4e4d-122">说明</span><span class="sxs-lookup"><span data-stu-id="a4e4d-122">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a4e4d-123">parentReference</span><span class="sxs-lookup"><span data-stu-id="a4e4d-123">parentReference</span></span> | [<span data-ttu-id="a4e4d-124">ItemReference</span><span class="sxs-lookup"><span data-stu-id="a4e4d-124">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="a4e4d-p103">可选。引用在其中创建副本的父项。</span><span class="sxs-lookup"><span data-stu-id="a4e4d-p103">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="a4e4d-127">name</span><span class="sxs-lookup"><span data-stu-id="a4e4d-127">name</span></span>            | <span data-ttu-id="a4e4d-128">string</span><span class="sxs-lookup"><span data-stu-id="a4e4d-128">string</span></span>                                         | <span data-ttu-id="a4e4d-p104">可选。副本的新名称。如果未提供新名称，将同一名称用作原始名称。</span><span class="sxs-lookup"><span data-stu-id="a4e4d-p104">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="a4e4d-132">**注意：**_parentReference_ 应包括目标文件夹的 `driveId` 和 `id` 参数。</span><span class="sxs-lookup"><span data-stu-id="a4e4d-132">**Note:** The _parentReference_ should include the `driveId` and `id` parameters for the target folder.</span></span>

## <a name="example"></a><span data-ttu-id="a4e4d-133">示例</span><span class="sxs-lookup"><span data-stu-id="a4e4d-133">Example</span></span>

<span data-ttu-id="a4e4d-134">本示例将由 `{item-id}` 标识的文件复制到使用 `driveId` 和 `id` 值标识的文件夹。</span><span class="sxs-lookup"><span data-stu-id="a4e4d-134">This example copies a file identified by `{item-id}` into a folder identified with a `driveId` and `id` value.</span></span>
<span data-ttu-id="a4e4d-135">该文件的新副本将被命名为 `contoso plan (copy).txt`。</span><span class="sxs-lookup"><span data-stu-id="a4e4d-135">The new copy of the file will be named `contoso plan (copy).txt`.</span></span>

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "driveId": "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    "id": "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
  },
  "name": "contoso plan (copy).txt"
}
```

## <a name="response"></a><span data-ttu-id="a4e4d-136">响应</span><span class="sxs-lookup"><span data-stu-id="a4e4d-136">Response</span></span>

<span data-ttu-id="a4e4d-137">返回有关如何在接受请求时[监视复制操作进度](/graph/long-running-actions-overview)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a4e4d-137">Returns details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="a4e4d-138">`Location` 头值提供的服务 URL 将返回复制操作的最新状态。</span><span class="sxs-lookup"><span data-stu-id="a4e4d-138">The value of the `Location` header provides a URL for a service that will return the current state of the copy operation.</span></span>
<span data-ttu-id="a4e4d-139">可以根据此信息[确定复制操作完成时间](/graph/long-running-actions-overview)。</span><span class="sxs-lookup"><span data-stu-id="a4e4d-139">You can use this info to [determine when the copy has finished](/graph/long-running-actions-overview).</span></span>

### <a name="remarks"></a><span data-ttu-id="a4e4d-140">备注</span><span class="sxs-lookup"><span data-stu-id="a4e4d-140">Remarks</span></span>

<span data-ttu-id="a4e4d-p107">在许多情况下，复制操作采用异步执行。API 响应仅指明复制操作获得接受还是遭到拒绝（比如说，由于目标文件名已被其他对象使用而遭到拒绝）。</span><span class="sxs-lookup"><span data-stu-id="a4e4d-p107">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->

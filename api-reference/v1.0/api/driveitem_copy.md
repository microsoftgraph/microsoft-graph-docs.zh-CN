---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "复制文件或文件夹"
ms.openlocfilehash: 6740091f887e42a14b2a42c99ee586af4254c473
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="copy-a-driveitem"></a><span data-ttu-id="17831-102">复制 DriveItem</span><span class="sxs-lookup"><span data-stu-id="17831-102">Copy a DriveItem</span></span>

<span data-ttu-id="17831-103">以异步方式在新父项下或使用新名称创建一个 [driveItem][item-resource] 副本（包括任何子级）。</span><span class="sxs-lookup"><span data-stu-id="17831-103">Creates a copy of a [driveItem] (including any children) under a new parent or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="17831-104">权限</span><span class="sxs-lookup"><span data-stu-id="17831-104">Permissions</span></span>

<span data-ttu-id="17831-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="17831-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="17831-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="17831-107">Permission type</span></span>      | <span data-ttu-id="17831-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17831-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17831-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17831-109">Delegated (work or school account)</span></span> | <span data-ttu-id="17831-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17831-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="17831-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17831-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17831-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17831-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="17831-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="17831-113">Application</span></span> | <span data-ttu-id="17831-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17831-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17831-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17831-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a><span data-ttu-id="17831-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="17831-116">Request body</span></span>

<span data-ttu-id="17831-117">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="17831-117">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="17831-118">名称</span><span class="sxs-lookup"><span data-stu-id="17831-118">Name</span></span>            | <span data-ttu-id="17831-119">值</span><span class="sxs-lookup"><span data-stu-id="17831-119">Value</span></span>                                          | <span data-ttu-id="17831-120">说明</span><span class="sxs-lookup"><span data-stu-id="17831-120">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="17831-121">parentReference</span><span class="sxs-lookup"><span data-stu-id="17831-121">parentReference</span></span> | [<span data-ttu-id="17831-122">ItemReference</span><span class="sxs-lookup"><span data-stu-id="17831-122">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="17831-p102">可选。引用在其中创建副本的父项。</span><span class="sxs-lookup"><span data-stu-id="17831-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="17831-125">name</span><span class="sxs-lookup"><span data-stu-id="17831-125">name</span></span>            | <span data-ttu-id="17831-126">string</span><span class="sxs-lookup"><span data-stu-id="17831-126">string</span></span>                                         | <span data-ttu-id="17831-p103">可选。副本的新名称。如果未提供新名称，将同一名称用作原始名称。</span><span class="sxs-lookup"><span data-stu-id="17831-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="17831-130">**注意：**_parentReference_ 应包括目标文件夹的 `driveId` 和 `id` 参数。</span><span class="sxs-lookup"><span data-stu-id="17831-130">**Note:** The _parentReference_ should include the `driveId` and `id` parameters for the target folder.</span></span>

## <a name="example"></a><span data-ttu-id="17831-131">示例</span><span class="sxs-lookup"><span data-stu-id="17831-131">Example</span></span>

<span data-ttu-id="17831-132">本示例将由 `{item-id}` 标识的文件复制到通过 `driveId` 和 `id` 值标识的文件夹。</span><span class="sxs-lookup"><span data-stu-id="17831-132">This example copies a file identified by `{item-id}` into a folder identified with a `driveId` and `id` value.</span></span>
<span data-ttu-id="17831-133">该文件的新副本将被命名为 `contoso plan (copy).txt`。</span><span class="sxs-lookup"><span data-stu-id="17831-133">The new copy of the file will be named `contoso plan (copy).txt`.</span></span>

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

## <a name="response"></a><span data-ttu-id="17831-134">响应</span><span class="sxs-lookup"><span data-stu-id="17831-134">Response</span></span>

<span data-ttu-id="17831-135">返回有关如何在接受请求时[监视复制操作进度](../../../concepts/long_running_actions_overview.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="17831-135">Returns details about how to [monitor the progress](../../../concepts/long_running_actions_overview.md) of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="17831-136">`Location` 头值提供的服务 URL 将返回复制操作的最新状态。</span><span class="sxs-lookup"><span data-stu-id="17831-136">The value of the `Location` header provides a URL for a service that will return the current state of the copy operation.</span></span>
<span data-ttu-id="17831-137">可以根据此信息[确定复制操作完成时间](../../../concepts/long_running_actions_overview.md)。</span><span class="sxs-lookup"><span data-stu-id="17831-137">You can use this info to [determine when the copy has finished](../../../concepts/long_running_actions_overview.md).</span></span>

### <a name="remarks"></a><span data-ttu-id="17831-138">备注</span><span class="sxs-lookup"><span data-stu-id="17831-138">Remarks</span></span>

<span data-ttu-id="17831-p106">在许多情况下，复制操作采用异步执行。API 响应仅指明复制操作获得接受还是遭到拒绝（比如说，由于目标文件名已被其他对象使用而遭到拒绝）。</span><span class="sxs-lookup"><span data-stu-id="17831-p106">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->

---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 签入文件
localization_priority: Normal
ms.openlocfilehash: 685bd89ed13bba4c4687620b00d346c7557214c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853923"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="9791d-102">签入对 DriveItem 资源的更改</span><span class="sxs-lookup"><span data-stu-id="9791d-102">Check-in changes to a DriveItem resource</span></span>

> <span data-ttu-id="9791d-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9791d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9791d-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9791d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9791d-105">签入已签出的 DriveItem 资源，为其他人提供文档版本。</span><span class="sxs-lookup"><span data-stu-id="9791d-105">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="9791d-106">权限</span><span class="sxs-lookup"><span data-stu-id="9791d-106">Permissions</span></span>

<span data-ttu-id="9791d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9791d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9791d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9791d-109">Permission type</span></span>      | <span data-ttu-id="9791d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9791d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9791d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9791d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9791d-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9791d-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9791d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9791d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9791d-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9791d-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="9791d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9791d-115">Application</span></span> | <span data-ttu-id="9791d-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9791d-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9791d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9791d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="9791d-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="9791d-118">Request body</span></span>

<span data-ttu-id="9791d-119">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9791d-119">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="9791d-120">名称</span><span class="sxs-lookup"><span data-stu-id="9791d-120">Name</span></span>    | <span data-ttu-id="9791d-121">值</span><span class="sxs-lookup"><span data-stu-id="9791d-121">Value</span></span>  |                                                <span data-ttu-id="9791d-122">说明</span><span class="sxs-lookup"><span data-stu-id="9791d-122">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9791d-123">checkInAs</span><span class="sxs-lookup"><span data-stu-id="9791d-123">checkInAs</span></span> | <span data-ttu-id="9791d-124">string</span><span class="sxs-lookup"><span data-stu-id="9791d-124">string</span></span> | <span data-ttu-id="9791d-125">可选。</span><span class="sxs-lookup"><span data-stu-id="9791d-125">Optional.</span></span> <span data-ttu-id="9791d-126">完成签入操作后文档的所需状态。</span><span class="sxs-lookup"><span data-stu-id="9791d-126">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="9791d-127">可以是 `published` 或未指定。</span><span class="sxs-lookup"><span data-stu-id="9791d-127">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="9791d-128">comment</span><span class="sxs-lookup"><span data-stu-id="9791d-128">comment</span></span>   | <span data-ttu-id="9791d-129">string</span><span class="sxs-lookup"><span data-stu-id="9791d-129">string</span></span> | <span data-ttu-id="9791d-130">与此版本相关联的签入注释。</span><span class="sxs-lookup"><span data-stu-id="9791d-130">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="9791d-131">示例</span><span class="sxs-lookup"><span data-stu-id="9791d-131">Example</span></span>

<span data-ttu-id="9791d-132">本示例签入由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="9791d-132">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="9791d-133">响应</span><span class="sxs-lookup"><span data-stu-id="9791d-133">Response</span></span>

<span data-ttu-id="9791d-134">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="9791d-134">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="9791d-135">注解</span><span class="sxs-lookup"><span data-stu-id="9791d-135">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->

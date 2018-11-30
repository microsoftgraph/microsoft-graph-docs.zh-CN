---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 签出文件
ms.openlocfilehash: c8b7cd9231150d9898ea21a15c4745791137cdba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042898"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="eac27-102">签出 DriveItem 资源</span><span class="sxs-lookup"><span data-stu-id="eac27-102">Check-out a DriveItem resource</span></span>

> <span data-ttu-id="eac27-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eac27-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eac27-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eac27-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eac27-105">签出 driveItem 资源以防止在[签入](driveitem-checkin.md)文档前其他人编辑文档和看到所做的更改。</span><span class="sxs-lookup"><span data-stu-id="eac27-105">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eac27-106">权限</span><span class="sxs-lookup"><span data-stu-id="eac27-106">Permissions</span></span>

<span data-ttu-id="eac27-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eac27-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eac27-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eac27-109">Permission type</span></span>      | <span data-ttu-id="eac27-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eac27-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eac27-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eac27-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eac27-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eac27-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="eac27-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eac27-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eac27-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eac27-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="eac27-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eac27-115">Application</span></span> | <span data-ttu-id="eac27-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eac27-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eac27-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eac27-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="eac27-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="eac27-118">Request body</span></span>

<span data-ttu-id="eac27-119">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="eac27-119">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="eac27-120">示例</span><span class="sxs-lookup"><span data-stu-id="eac27-120">Example</span></span>

<span data-ttu-id="eac27-121">本示例签出由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="eac27-121">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="eac27-122">响应</span><span class="sxs-lookup"><span data-stu-id="eac27-122">Response</span></span>

<span data-ttu-id="eac27-123">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="eac27-123">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="eac27-124">注解</span><span class="sxs-lookup"><span data-stu-id="eac27-124">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->

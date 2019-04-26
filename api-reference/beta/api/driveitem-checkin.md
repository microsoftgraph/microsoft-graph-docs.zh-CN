---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 签入文件
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: cec932eef89c02569d6f350f436c6a7721286e92
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325401"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="9416e-102">签入对 DriveItem 资源的更改</span><span class="sxs-lookup"><span data-stu-id="9416e-102">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9416e-103">签入已签出的 DriveItem 资源，为其他人提供文档版本。</span><span class="sxs-lookup"><span data-stu-id="9416e-103">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="9416e-104">权限</span><span class="sxs-lookup"><span data-stu-id="9416e-104">Permissions</span></span>

<span data-ttu-id="9416e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9416e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9416e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="9416e-107">Permission type</span></span>      | <span data-ttu-id="9416e-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9416e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9416e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9416e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9416e-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9416e-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9416e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9416e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9416e-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9416e-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="9416e-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="9416e-113">Application</span></span> | <span data-ttu-id="9416e-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9416e-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9416e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9416e-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="9416e-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="9416e-116">Request body</span></span>

<span data-ttu-id="9416e-117">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9416e-117">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="9416e-118">名称</span><span class="sxs-lookup"><span data-stu-id="9416e-118">Name</span></span>    | <span data-ttu-id="9416e-119">值</span><span class="sxs-lookup"><span data-stu-id="9416e-119">Value</span></span>  |                                                <span data-ttu-id="9416e-120">说明</span><span class="sxs-lookup"><span data-stu-id="9416e-120">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9416e-121">checkInAs</span><span class="sxs-lookup"><span data-stu-id="9416e-121">checkInAs</span></span> | <span data-ttu-id="9416e-122">字符串</span><span class="sxs-lookup"><span data-stu-id="9416e-122">string</span></span> | <span data-ttu-id="9416e-123">可选。</span><span class="sxs-lookup"><span data-stu-id="9416e-123">Optional.</span></span> <span data-ttu-id="9416e-124">完成签入操作后文档的所需状态。</span><span class="sxs-lookup"><span data-stu-id="9416e-124">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="9416e-125">可以是 `published` 或未指定。</span><span class="sxs-lookup"><span data-stu-id="9416e-125">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="9416e-126">comment</span><span class="sxs-lookup"><span data-stu-id="9416e-126">comment</span></span>   | <span data-ttu-id="9416e-127">string</span><span class="sxs-lookup"><span data-stu-id="9416e-127">string</span></span> | <span data-ttu-id="9416e-128">与此版本相关联的签入注释。</span><span class="sxs-lookup"><span data-stu-id="9416e-128">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="9416e-129">示例</span><span class="sxs-lookup"><span data-stu-id="9416e-129">Example</span></span>

<span data-ttu-id="9416e-130">本示例签入由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="9416e-130">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="9416e-131">响应</span><span class="sxs-lookup"><span data-stu-id="9416e-131">Response</span></span>

<span data-ttu-id="9416e-132">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="9416e-132">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="9416e-133">注解</span><span class="sxs-lookup"><span data-stu-id="9416e-133">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": []
}
-->

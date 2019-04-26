---
title: 'mailFolder: move'
description: 将 Mailfolder 及其内容移动到其他 mailfolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 68b871a188be207f3e9cede7f48cb6bea36ebafd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338668"
---
# <a name="mailfolder-move"></a><span data-ttu-id="1e354-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="1e354-103">mailFolder: move</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e354-104">将 Mailfolder 及其内容移动到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="1e354-104">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e354-105">权限</span><span class="sxs-lookup"><span data-stu-id="1e354-105">Permissions</span></span>

<span data-ttu-id="1e354-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e354-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1e354-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e354-108">Permission type</span></span> | <span data-ttu-id="1e354-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e354-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="1e354-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e354-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e354-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e354-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1e354-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e354-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e354-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e354-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1e354-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e354-114">Application</span></span> | <span data-ttu-id="1e354-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e354-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e354-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e354-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="1e354-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e354-117">Request headers</span></span>

| <span data-ttu-id="1e354-118">标头</span><span class="sxs-lookup"><span data-stu-id="1e354-118">Header</span></span> | <span data-ttu-id="1e354-119">值</span><span class="sxs-lookup"><span data-stu-id="1e354-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="1e354-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e354-120">Authorization</span></span> | <span data-ttu-id="1e354-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="1e354-121"></span></span> <span data-ttu-id="1e354-122">必需。</span><span class="sxs-lookup"><span data-stu-id="1e354-122">Required.</span></span> |
| <span data-ttu-id="1e354-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1e354-123">Content-Type</span></span> | <span data-ttu-id="1e354-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="1e354-124"></span></span> <span data-ttu-id="1e354-125">必需。</span><span class="sxs-lookup"><span data-stu-id="1e354-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e354-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e354-126">Request body</span></span>

<span data-ttu-id="1e354-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1e354-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1e354-128">参数</span><span class="sxs-lookup"><span data-stu-id="1e354-128">Parameter</span></span> | <span data-ttu-id="1e354-129">类型</span><span class="sxs-lookup"><span data-stu-id="1e354-129">Type</span></span> | <span data-ttu-id="1e354-130">说明</span><span class="sxs-lookup"><span data-stu-id="1e354-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="1e354-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="1e354-131">destinationId</span></span>|<span data-ttu-id="1e354-132">String</span><span class="sxs-lookup"><span data-stu-id="1e354-132">String</span></span>|<span data-ttu-id="1e354-133">文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="1e354-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="1e354-134">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="1e354-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="1e354-135">响应</span><span class="sxs-lookup"><span data-stu-id="1e354-135">Response</span></span>

<span data-ttu-id="1e354-136">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[mailFolder](../resources/mailfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1e354-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e354-137">示例</span><span class="sxs-lookup"><span data-stu-id="1e354-137">Example</span></span>

<span data-ttu-id="1e354-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1e354-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1e354-139">请求</span><span class="sxs-lookup"><span data-stu-id="1e354-139">Request</span></span>

<span data-ttu-id="1e354-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e354-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="1e354-141">响应</span><span class="sxs-lookup"><span data-stu-id="1e354-141">Response</span></span>

<span data-ttu-id="1e354-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1e354-142">Here is an example of the response.</span></span>

> <span data-ttu-id="1e354-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1e354-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1e354-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1e354-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

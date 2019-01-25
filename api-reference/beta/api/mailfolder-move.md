---
title: 'mailFolder: move'
description: 将 Mailfolder 及其内容移动到其他 mailfolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 836c91ee2bfd234c5c831511d1be45800be8660a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512127"
---
# <a name="mailfolder-move"></a><span data-ttu-id="d0dc3-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="d0dc3-103">mailFolder: move</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0dc3-104">将 Mailfolder 及其内容移动到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="d0dc3-104">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0dc3-105">权限</span><span class="sxs-lookup"><span data-stu-id="d0dc3-105">Permissions</span></span>

<span data-ttu-id="d0dc3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0dc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0dc3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0dc3-108">Permission type</span></span> | <span data-ttu-id="d0dc3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0dc3-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="d0dc3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0dc3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d0dc3-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0dc3-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d0dc3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0dc3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0dc3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0dc3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d0dc3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0dc3-114">Application</span></span> | <span data-ttu-id="d0dc3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0dc3-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0dc3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0dc3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="d0dc3-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0dc3-117">Request headers</span></span>

| <span data-ttu-id="d0dc3-118">标头</span><span class="sxs-lookup"><span data-stu-id="d0dc3-118">Header</span></span> | <span data-ttu-id="d0dc3-119">值</span><span class="sxs-lookup"><span data-stu-id="d0dc3-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="d0dc3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0dc3-120">Authorization</span></span> | <span data-ttu-id="d0dc3-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="d0dc3-121"></span></span> <span data-ttu-id="d0dc3-122">必需。</span><span class="sxs-lookup"><span data-stu-id="d0dc3-122">Required.</span></span> |
| <span data-ttu-id="d0dc3-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0dc3-123">Content-Type</span></span> | <span data-ttu-id="d0dc3-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="d0dc3-124"></span></span> <span data-ttu-id="d0dc3-125">必需。</span><span class="sxs-lookup"><span data-stu-id="d0dc3-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0dc3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0dc3-126">Request body</span></span>

<span data-ttu-id="d0dc3-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d0dc3-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d0dc3-128">参数</span><span class="sxs-lookup"><span data-stu-id="d0dc3-128">Parameter</span></span> | <span data-ttu-id="d0dc3-129">类型</span><span class="sxs-lookup"><span data-stu-id="d0dc3-129">Type</span></span> | <span data-ttu-id="d0dc3-130">说明</span><span class="sxs-lookup"><span data-stu-id="d0dc3-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="d0dc3-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="d0dc3-131">destinationId</span></span>|<span data-ttu-id="d0dc3-132">String</span><span class="sxs-lookup"><span data-stu-id="d0dc3-132">String</span></span>|<span data-ttu-id="d0dc3-133">文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="d0dc3-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="d0dc3-134">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="d0dc3-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="d0dc3-135">响应</span><span class="sxs-lookup"><span data-stu-id="d0dc3-135">Response</span></span>

<span data-ttu-id="d0dc3-136">如果成功，此方法返回`200 OK`响应代码和响应正文中的[mailFolder](../resources/mailfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d0dc3-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0dc3-137">示例</span><span class="sxs-lookup"><span data-stu-id="d0dc3-137">Example</span></span>

<span data-ttu-id="d0dc3-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d0dc3-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d0dc3-139">请求</span><span class="sxs-lookup"><span data-stu-id="d0dc3-139">Request</span></span>

<span data-ttu-id="d0dc3-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0dc3-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d0dc3-141">响应</span><span class="sxs-lookup"><span data-stu-id="d0dc3-141">Response</span></span>

<span data-ttu-id="d0dc3-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d0dc3-142">Here is an example of the response.</span></span>

> <span data-ttu-id="d0dc3-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d0dc3-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d0dc3-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d0dc3-144">All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-move.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

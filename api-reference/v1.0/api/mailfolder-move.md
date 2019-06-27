---
title: 'mailFolder: move'
description: 将 Mailfolder 及其内容移动到其他 mailfolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8449b85fe4c535641ea38397bfe580437e7d29fe
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277243"
---
# <a name="mailfolder-move"></a><span data-ttu-id="d618f-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="d618f-103">mailFolder: move</span></span>

<span data-ttu-id="d618f-104">将 Mailfolder 及其内容移动到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="d618f-104">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="d618f-105">权限</span><span class="sxs-lookup"><span data-stu-id="d618f-105">Permissions</span></span>

<span data-ttu-id="d618f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d618f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d618f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d618f-108">Permission type</span></span> | <span data-ttu-id="d618f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d618f-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="d618f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d618f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d618f-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d618f-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d618f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d618f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d618f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d618f-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d618f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d618f-114">Application</span></span> | <span data-ttu-id="d618f-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d618f-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d618f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d618f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="d618f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d618f-117">Request headers</span></span>

| <span data-ttu-id="d618f-118">标头</span><span class="sxs-lookup"><span data-stu-id="d618f-118">Header</span></span> | <span data-ttu-id="d618f-119">值</span><span class="sxs-lookup"><span data-stu-id="d618f-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="d618f-120">授权</span><span class="sxs-lookup"><span data-stu-id="d618f-120">Authorization</span></span> | <span data-ttu-id="d618f-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="d618f-121"></span></span> <span data-ttu-id="d618f-122">必需。</span><span class="sxs-lookup"><span data-stu-id="d618f-122">Required.</span></span> |
| <span data-ttu-id="d618f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d618f-123">Content-Type</span></span> | <span data-ttu-id="d618f-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="d618f-124"></span></span> <span data-ttu-id="d618f-125">必需。</span><span class="sxs-lookup"><span data-stu-id="d618f-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d618f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d618f-126">Request body</span></span>

<span data-ttu-id="d618f-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d618f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d618f-128">参数</span><span class="sxs-lookup"><span data-stu-id="d618f-128">Parameter</span></span> | <span data-ttu-id="d618f-129">类型</span><span class="sxs-lookup"><span data-stu-id="d618f-129">Type</span></span> | <span data-ttu-id="d618f-130">说明</span><span class="sxs-lookup"><span data-stu-id="d618f-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="d618f-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="d618f-131">destinationId</span></span>|<span data-ttu-id="d618f-132">String</span><span class="sxs-lookup"><span data-stu-id="d618f-132">String</span></span>|<span data-ttu-id="d618f-133">文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="d618f-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="d618f-134">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="d618f-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="d618f-135">响应</span><span class="sxs-lookup"><span data-stu-id="d618f-135">Response</span></span>

<span data-ttu-id="d618f-136">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[mailFolder](../resources/mailfolder.md)资源。</span><span class="sxs-lookup"><span data-stu-id="d618f-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d618f-137">示例</span><span class="sxs-lookup"><span data-stu-id="d618f-137">Example</span></span>

<span data-ttu-id="d618f-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d618f-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d618f-139">请求</span><span class="sxs-lookup"><span data-stu-id="d618f-139">Request</span></span>

<span data-ttu-id="d618f-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d618f-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="d618f-141">响应</span><span class="sxs-lookup"><span data-stu-id="d618f-141">Response</span></span>

<span data-ttu-id="d618f-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d618f-142">Here is an example of the response.</span></span>

> <span data-ttu-id="d618f-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d618f-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d618f-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d618f-144">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d618f-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d618f-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d618f-146">C#</span><span class="sxs-lookup"><span data-stu-id="d618f-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/mailfolder_move-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d618f-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="d618f-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/mailfolder_move-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d618f-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="d618f-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/mailfolder_move-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-move.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/mailfolder-move.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-move.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

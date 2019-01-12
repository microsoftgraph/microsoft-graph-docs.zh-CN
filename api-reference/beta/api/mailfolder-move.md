---
title: 'mailFolder: move'
description: 将 Mailfolder 及其内容移动到其他 mailfolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fc43041fa8d6d2b4c498d7ab40f850e103e741d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951087"
---
# <a name="mailfolder-move"></a><span data-ttu-id="32e55-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="32e55-103">mailFolder: move</span></span>

> <span data-ttu-id="32e55-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="32e55-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32e55-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="32e55-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32e55-106">将 Mailfolder 及其内容移动到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="32e55-106">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="32e55-107">权限</span><span class="sxs-lookup"><span data-stu-id="32e55-107">Permissions</span></span>

<span data-ttu-id="32e55-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32e55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32e55-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="32e55-110">Permission type</span></span> | <span data-ttu-id="32e55-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32e55-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="32e55-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32e55-112">Delegated (work or school account)</span></span> | <span data-ttu-id="32e55-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32e55-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="32e55-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32e55-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32e55-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32e55-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="32e55-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="32e55-116">Application</span></span> | <span data-ttu-id="32e55-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32e55-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="32e55-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32e55-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="32e55-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="32e55-119">Request headers</span></span>

| <span data-ttu-id="32e55-120">标头</span><span class="sxs-lookup"><span data-stu-id="32e55-120">Header</span></span> | <span data-ttu-id="32e55-121">值</span><span class="sxs-lookup"><span data-stu-id="32e55-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="32e55-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="32e55-122">Authorization</span></span> | <span data-ttu-id="32e55-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="32e55-123"></span></span> <span data-ttu-id="32e55-124">必填。</span><span class="sxs-lookup"><span data-stu-id="32e55-124">Required.</span></span> |
| <span data-ttu-id="32e55-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32e55-125">Content-Type</span></span> | <span data-ttu-id="32e55-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="32e55-126"></span></span> <span data-ttu-id="32e55-127">必填。</span><span class="sxs-lookup"><span data-stu-id="32e55-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32e55-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="32e55-128">Request body</span></span>

<span data-ttu-id="32e55-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="32e55-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="32e55-130">参数</span><span class="sxs-lookup"><span data-stu-id="32e55-130">Parameter</span></span> | <span data-ttu-id="32e55-131">类型</span><span class="sxs-lookup"><span data-stu-id="32e55-131">Type</span></span> | <span data-ttu-id="32e55-132">说明</span><span class="sxs-lookup"><span data-stu-id="32e55-132">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="32e55-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="32e55-133">destinationId</span></span>|<span data-ttu-id="32e55-134">字符串</span><span class="sxs-lookup"><span data-stu-id="32e55-134">String</span></span>|<span data-ttu-id="32e55-135">文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="32e55-135">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="32e55-136">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="32e55-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="32e55-137">响应</span><span class="sxs-lookup"><span data-stu-id="32e55-137">Response</span></span>

<span data-ttu-id="32e55-138">如果成功，此方法返回`200 OK`响应代码和响应正文中的[mailFolder](../resources/mailfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="32e55-138">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32e55-139">示例</span><span class="sxs-lookup"><span data-stu-id="32e55-139">Example</span></span>

<span data-ttu-id="32e55-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="32e55-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="32e55-141">请求</span><span class="sxs-lookup"><span data-stu-id="32e55-141">Request</span></span>

<span data-ttu-id="32e55-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="32e55-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="32e55-143">响应</span><span class="sxs-lookup"><span data-stu-id="32e55-143">Response</span></span>

<span data-ttu-id="32e55-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="32e55-144">Here is an example of the response.</span></span>

> <span data-ttu-id="32e55-145">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="32e55-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="32e55-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="32e55-146">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

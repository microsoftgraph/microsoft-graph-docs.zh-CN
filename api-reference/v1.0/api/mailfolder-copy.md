---
title: 'mailFolder: copy'
description: 将 mailfolder 及其内容复制到其他 mailfolder。
author: angelgolfer-ms
ms.openlocfilehash: 44df53219e00479cdc48d057286f1af410e13c77
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356923"
---
# <a name="mailfolder-copy"></a><span data-ttu-id="ae6dd-103">mailFolder: copy</span><span class="sxs-lookup"><span data-stu-id="ae6dd-103">mailFolder: copy</span></span>

<span data-ttu-id="ae6dd-104">将 mailfolder 及其内容复制到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="ae6dd-104">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae6dd-105">权限</span><span class="sxs-lookup"><span data-stu-id="ae6dd-105">Permissions</span></span>

<span data-ttu-id="ae6dd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae6dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae6dd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae6dd-108">Permission type</span></span> | <span data-ttu-id="ae6dd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae6dd-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="ae6dd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae6dd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae6dd-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae6dd-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ae6dd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae6dd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae6dd-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae6dd-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ae6dd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae6dd-114">Application</span></span> | <span data-ttu-id="ae6dd-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae6dd-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae6dd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae6dd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="ae6dd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae6dd-117">Request headers</span></span>
| <span data-ttu-id="ae6dd-118">标头</span><span class="sxs-lookup"><span data-stu-id="ae6dd-118">Header</span></span> | <span data-ttu-id="ae6dd-119">值</span><span class="sxs-lookup"><span data-stu-id="ae6dd-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="ae6dd-120">授权</span><span class="sxs-lookup"><span data-stu-id="ae6dd-120">Authorization</span></span> | <span data-ttu-id="ae6dd-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="ae6dd-121"></span></span> <span data-ttu-id="ae6dd-122">必需。</span><span class="sxs-lookup"><span data-stu-id="ae6dd-122">Required.</span></span> |
| <span data-ttu-id="ae6dd-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae6dd-123">Content-Type</span></span> | <span data-ttu-id="ae6dd-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="ae6dd-124"></span></span> <span data-ttu-id="ae6dd-125">必需。</span><span class="sxs-lookup"><span data-stu-id="ae6dd-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae6dd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae6dd-126">Request body</span></span>

<span data-ttu-id="ae6dd-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ae6dd-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ae6dd-128">参数</span><span class="sxs-lookup"><span data-stu-id="ae6dd-128">Parameter</span></span> | <span data-ttu-id="ae6dd-129">Type</span><span class="sxs-lookup"><span data-stu-id="ae6dd-129">Type</span></span> | <span data-ttu-id="ae6dd-130">说明</span><span class="sxs-lookup"><span data-stu-id="ae6dd-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="ae6dd-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="ae6dd-131">destinationId</span></span>|<span data-ttu-id="ae6dd-132">字符串</span><span class="sxs-lookup"><span data-stu-id="ae6dd-132">String</span></span>|<span data-ttu-id="ae6dd-133">文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="ae6dd-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="ae6dd-134">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="ae6dd-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="ae6dd-135">响应</span><span class="sxs-lookup"><span data-stu-id="ae6dd-135">Response</span></span>

<span data-ttu-id="ae6dd-136">如果成功，此方法返回`200 OK`响应代码和响应正文的[mailFolder](../resources/mailfolder.md)资源。</span><span class="sxs-lookup"><span data-stu-id="ae6dd-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae6dd-137">示例</span><span class="sxs-lookup"><span data-stu-id="ae6dd-137">Example</span></span>

<span data-ttu-id="ae6dd-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ae6dd-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ae6dd-139">请求</span><span class="sxs-lookup"><span data-stu-id="ae6dd-139">Request</span></span>
<span data-ttu-id="ae6dd-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ae6dd-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="ae6dd-141">响应</span><span class="sxs-lookup"><span data-stu-id="ae6dd-141">Response</span></span>

<span data-ttu-id="ae6dd-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ae6dd-142">Here is an example of the response.</span></span>

> <span data-ttu-id="ae6dd-143">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ae6dd-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ae6dd-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ae6dd-144">All the properties will be returned from an actual call.</span></span>
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
  "description": "mailFolder: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

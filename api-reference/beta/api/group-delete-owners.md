---
title: 删除所有者
description: 使用此 API 可以通过 owners 导航属性从 Office 365 组、安全组或启用邮件的安全组中删除所有者。
localization_priority: Normal
ms.openlocfilehash: af45706e6f42f3442e28dd8a04fe6863f957a6fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843356"
---
# <a name="remove-owner"></a><span data-ttu-id="3e70c-103">删除所有者</span><span class="sxs-lookup"><span data-stu-id="3e70c-103">Remove owner</span></span>

> <span data-ttu-id="3e70c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3e70c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e70c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3e70c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e70c-106">使用此 API 可以通过 owners 导航属性从 Office 365 组、安全组或启用邮件的安全组中删除所有者。</span><span class="sxs-lookup"><span data-stu-id="3e70c-106">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e70c-107">权限</span><span class="sxs-lookup"><span data-stu-id="3e70c-107">Permissions</span></span>
<span data-ttu-id="3e70c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e70c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e70c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e70c-110">Permission type</span></span>      | <span data-ttu-id="3e70c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e70c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e70c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e70c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e70c-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3e70c-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3e70c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e70c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e70c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e70c-115">Not supported.</span></span>    |
|<span data-ttu-id="3e70c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e70c-116">Application</span></span> | <span data-ttu-id="3e70c-117">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e70c-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e70c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e70c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="3e70c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e70c-119">Request headers</span></span>
| <span data-ttu-id="3e70c-120">名称</span><span class="sxs-lookup"><span data-stu-id="3e70c-120">Name</span></span>       | <span data-ttu-id="3e70c-121">类型</span><span class="sxs-lookup"><span data-stu-id="3e70c-121">Type</span></span> | <span data-ttu-id="3e70c-122">说明</span><span class="sxs-lookup"><span data-stu-id="3e70c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3e70c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e70c-123">Authorization</span></span>  | <span data-ttu-id="3e70c-124">string</span><span class="sxs-lookup"><span data-stu-id="3e70c-124">string</span></span>  | <span data-ttu-id="3e70c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e70c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e70c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e70c-127">Request body</span></span>
<span data-ttu-id="3e70c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3e70c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e70c-129">响应</span><span class="sxs-lookup"><span data-stu-id="3e70c-129">Response</span></span>
<span data-ttu-id="3e70c-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3e70c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e70c-132">示例</span><span class="sxs-lookup"><span data-stu-id="3e70c-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3e70c-133">请求</span><span class="sxs-lookup"><span data-stu-id="3e70c-133">Request</span></span>
<span data-ttu-id="3e70c-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3e70c-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="3e70c-135">在请求中，指定要在 $ref 段后删除的 directory 对象 `id`。</span><span class="sxs-lookup"><span data-stu-id="3e70c-135">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="3e70c-136">响应</span><span class="sxs-lookup"><span data-stu-id="3e70c-136">Response</span></span>
<span data-ttu-id="3e70c-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3e70c-137">The following is an example of the response.</span></span>
><span data-ttu-id="3e70c-138">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3e70c-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3e70c-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3e70c-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

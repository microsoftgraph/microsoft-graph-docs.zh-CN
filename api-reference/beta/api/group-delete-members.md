---
title: 删除成员
description: 使用此 API 可以通过 **members** 导航属性从 Office 365 组、安全组或启用邮件的安全组中删除成员。可以删除用户或其他组。
localization_priority: Normal
ms.openlocfilehash: 917e662158785111847d5d74821bfedbb61205dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864475"
---
# <a name="remove-member"></a><span data-ttu-id="5367d-104">删除成员</span><span class="sxs-lookup"><span data-stu-id="5367d-104">Remove member</span></span>

> <span data-ttu-id="5367d-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5367d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5367d-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5367d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5367d-p103">使用此 API 可以通过 **members** 导航属性从 Office 365 组、安全组或启用邮件的安全组中删除成员。可以删除用户或其他组。</span><span class="sxs-lookup"><span data-stu-id="5367d-p103">Use this API to remove a member from an Office 365 group, a security group, or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="5367d-109">权限</span><span class="sxs-lookup"><span data-stu-id="5367d-109">Permissions</span></span>
<span data-ttu-id="5367d-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5367d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5367d-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5367d-112">Permission type</span></span>      | <span data-ttu-id="5367d-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5367d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5367d-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5367d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5367d-115">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5367d-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5367d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5367d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5367d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5367d-117">Not supported.</span></span>    |
|<span data-ttu-id="5367d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5367d-118">Application</span></span> | <span data-ttu-id="5367d-119">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5367d-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5367d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5367d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5367d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5367d-121">Request headers</span></span>
| <span data-ttu-id="5367d-122">名称</span><span class="sxs-lookup"><span data-stu-id="5367d-122">Name</span></span>       | <span data-ttu-id="5367d-123">类型</span><span class="sxs-lookup"><span data-stu-id="5367d-123">Type</span></span> | <span data-ttu-id="5367d-124">说明</span><span class="sxs-lookup"><span data-stu-id="5367d-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5367d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5367d-125">Authorization</span></span>  | <span data-ttu-id="5367d-126">string</span><span class="sxs-lookup"><span data-stu-id="5367d-126">string</span></span>  | <span data-ttu-id="5367d-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5367d-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5367d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5367d-129">Request body</span></span>
<span data-ttu-id="5367d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5367d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5367d-131">响应</span><span class="sxs-lookup"><span data-stu-id="5367d-131">Response</span></span>
<span data-ttu-id="5367d-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5367d-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5367d-134">示例</span><span class="sxs-lookup"><span data-stu-id="5367d-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5367d-135">请求</span><span class="sxs-lookup"><span data-stu-id="5367d-135">Request</span></span>
<span data-ttu-id="5367d-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5367d-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="5367d-137">在请求中，指定要在 $ref 段后删除的 directory 对象 `id`。</span><span class="sxs-lookup"><span data-stu-id="5367d-137">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="5367d-138">响应</span><span class="sxs-lookup"><span data-stu-id="5367d-138">Response</span></span>
<span data-ttu-id="5367d-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5367d-139">The following is an example of the response.</span></span>
><span data-ttu-id="5367d-140">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5367d-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5367d-141">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5367d-141">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

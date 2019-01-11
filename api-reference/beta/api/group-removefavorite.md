---
title: 'group: removeFavorite'
description: 从当前用户收藏夹组列表中删除组。仅支持 Office 365 组。
localization_priority: Normal
ms.openlocfilehash: 7299c89bc95ce267adf0149cbf3ff3f76c3a52ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887260"
---
# <a name="group-removefavorite"></a><span data-ttu-id="f64a2-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="f64a2-104">group: removeFavorite</span></span>

> <span data-ttu-id="f64a2-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f64a2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f64a2-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f64a2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f64a2-p103">从当前用户收藏夹组列表中删除组。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="f64a2-p103">Remove the group from the list of the current user's favorite groups. Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="f64a2-109">权限</span><span class="sxs-lookup"><span data-stu-id="f64a2-109">Permissions</span></span>
<span data-ttu-id="f64a2-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f64a2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f64a2-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f64a2-112">Permission type</span></span>      | <span data-ttu-id="f64a2-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f64a2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f64a2-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f64a2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f64a2-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f64a2-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f64a2-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f64a2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f64a2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f64a2-117">Not supported.</span></span>    |
|<span data-ttu-id="f64a2-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f64a2-118">Application</span></span> | <span data-ttu-id="f64a2-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f64a2-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f64a2-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f64a2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```

## <a name="request-headers"></a><span data-ttu-id="f64a2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f64a2-121">Request headers</span></span>
| <span data-ttu-id="f64a2-122">标头</span><span class="sxs-lookup"><span data-stu-id="f64a2-122">Header</span></span>       | <span data-ttu-id="f64a2-123">值</span><span class="sxs-lookup"><span data-stu-id="f64a2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f64a2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f64a2-124">Authorization</span></span>  | <span data-ttu-id="f64a2-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f64a2-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f64a2-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="f64a2-127">Prefer</span></span> | <span data-ttu-id="f64a2-128">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="f64a2-128">return=minimal.</span></span> <span data-ttu-id="f64a2-129">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="f64a2-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="f64a2-130">可选。</span><span class="sxs-lookup"><span data-stu-id="f64a2-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="f64a2-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="f64a2-131">Request body</span></span>
<span data-ttu-id="f64a2-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f64a2-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f64a2-133">响应</span><span class="sxs-lookup"><span data-stu-id="f64a2-133">Response</span></span>
<span data-ttu-id="f64a2-p107">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f64a2-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f64a2-136">示例</span><span class="sxs-lookup"><span data-stu-id="f64a2-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f64a2-137">请求</span><span class="sxs-lookup"><span data-stu-id="f64a2-137">Request</span></span>
<span data-ttu-id="f64a2-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f64a2-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/removeFavorite
```

#### <a name="response"></a><span data-ttu-id="f64a2-139">响应</span><span class="sxs-lookup"><span data-stu-id="f64a2-139">Response</span></span>
<span data-ttu-id="f64a2-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f64a2-140">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

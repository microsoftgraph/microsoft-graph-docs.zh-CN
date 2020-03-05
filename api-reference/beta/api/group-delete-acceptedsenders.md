---
title: 删除 acceptedSender
description: '从接受的发件人列表中删除用户或组。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f4b82ccaef290efa0bec00785e5f1ad3a30f516f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42420575"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="abb3e-103">删除 acceptedSender</span><span class="sxs-lookup"><span data-stu-id="abb3e-103">Remove acceptedSender</span></span>

<span data-ttu-id="abb3e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="abb3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abb3e-105">从指定组的 "接受-发件人" 列表中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="abb3e-105">Remove a user or group from the accepted-senders list of the specified group.</span></span> 

## <a name="permissions"></a><span data-ttu-id="abb3e-106">权限</span><span class="sxs-lookup"><span data-stu-id="abb3e-106">Permissions</span></span>
<span data-ttu-id="abb3e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="abb3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="abb3e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="abb3e-109">Permission type</span></span>                        | <span data-ttu-id="abb3e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="abb3e-110">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="abb3e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="abb3e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="abb3e-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abb3e-112">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="abb3e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="abb3e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abb3e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="abb3e-114">Not supported.</span></span>|
| <span data-ttu-id="abb3e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="abb3e-115">Application</span></span>                            | <span data-ttu-id="abb3e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="abb3e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abb3e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="abb3e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="abb3e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="abb3e-118">Request headers</span></span>
| <span data-ttu-id="abb3e-119">标头</span><span class="sxs-lookup"><span data-stu-id="abb3e-119">Header</span></span>         | <span data-ttu-id="abb3e-120">值</span><span class="sxs-lookup"><span data-stu-id="abb3e-120">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="abb3e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="abb3e-121">Authorization</span></span>  | <span data-ttu-id="abb3e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="abb3e-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="abb3e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="abb3e-124">Request body</span></span>
<span data-ttu-id="abb3e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="abb3e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abb3e-126">响应</span><span class="sxs-lookup"><span data-stu-id="abb3e-126">Response</span></span>
<span data-ttu-id="abb3e-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="abb3e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="abb3e-129">示例</span><span class="sxs-lookup"><span data-stu-id="abb3e-129">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="abb3e-130">示例1：从组的接受-发件人列表中删除用户。</span><span class="sxs-lookup"><span data-stu-id="abb3e-130">Example 1: Remove a user from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="abb3e-131">请求</span><span class="sxs-lookup"><span data-stu-id="abb3e-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="abb3e-132">响应</span><span class="sxs-lookup"><span data-stu-id="abb3e-132">Response</span></span>
<span data-ttu-id="abb3e-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="abb3e-133">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "remove_user_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="abb3e-134">示例2：从组的 "接受-发件人" 列表中删除组。</span><span class="sxs-lookup"><span data-stu-id="abb3e-134">Example 2: Remove a group from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="abb3e-135">请求</span><span class="sxs-lookup"><span data-stu-id="abb3e-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_group_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="abb3e-136">响应</span><span class="sxs-lookup"><span data-stu-id="abb3e-136">Response</span></span>
<span data-ttu-id="abb3e-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="abb3e-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "remove_group_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

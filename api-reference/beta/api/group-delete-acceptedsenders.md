---
title: 删除 acceptedSender
description: '从接受的发件人列表中删除用户或组。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 22e81f8bbbb497b8209e6faa744a54b24029391c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329740"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="347f0-103">删除 acceptedSender</span><span class="sxs-lookup"><span data-stu-id="347f0-103">Remove acceptedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="347f0-104">从指定组的 "接受-发件人" 列表中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="347f0-104">Remove a user or group from the accepted-senders list of the specified group.</span></span> 

## <a name="permissions"></a><span data-ttu-id="347f0-105">权限</span><span class="sxs-lookup"><span data-stu-id="347f0-105">Permissions</span></span>
<span data-ttu-id="347f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="347f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="347f0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="347f0-108">Permission type</span></span>                        | <span data-ttu-id="347f0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="347f0-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="347f0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="347f0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="347f0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="347f0-111">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="347f0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="347f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="347f0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="347f0-113">Not supported.</span></span>|
| <span data-ttu-id="347f0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="347f0-114">Application</span></span>                            | <span data-ttu-id="347f0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="347f0-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="347f0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="347f0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="347f0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="347f0-117">Request headers</span></span>
| <span data-ttu-id="347f0-118">标头</span><span class="sxs-lookup"><span data-stu-id="347f0-118">Header</span></span>         | <span data-ttu-id="347f0-119">值</span><span class="sxs-lookup"><span data-stu-id="347f0-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="347f0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="347f0-120">Authorization</span></span>  | <span data-ttu-id="347f0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="347f0-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="347f0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="347f0-123">Request body</span></span>
<span data-ttu-id="347f0-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="347f0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="347f0-125">响应</span><span class="sxs-lookup"><span data-stu-id="347f0-125">Response</span></span>
<span data-ttu-id="347f0-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="347f0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="347f0-128">示例</span><span class="sxs-lookup"><span data-stu-id="347f0-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="347f0-129">示例 1: 从组的接受-发件人列表中删除用户。</span><span class="sxs-lookup"><span data-stu-id="347f0-129">Example 1: Remove a user from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="347f0-130">请求</span><span class="sxs-lookup"><span data-stu-id="347f0-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="347f0-131">响应</span><span class="sxs-lookup"><span data-stu-id="347f0-131">Response</span></span>
<span data-ttu-id="347f0-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="347f0-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "remove_user_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="347f0-133">示例 2: 从组的 "接受-发件人" 列表中删除组。</span><span class="sxs-lookup"><span data-stu-id="347f0-133">Example 2: Remove a group from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="347f0-134">请求</span><span class="sxs-lookup"><span data-stu-id="347f0-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_group_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="347f0-135">响应</span><span class="sxs-lookup"><span data-stu-id="347f0-135">Response</span></span>
<span data-ttu-id="347f0-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="347f0-136">The following is an example of the response.</span></span> 

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

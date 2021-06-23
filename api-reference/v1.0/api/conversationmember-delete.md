---
title: 删除 conversationMember
description: 从频道中删除 conversationMember。
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2b0489387f4822296788c417536332c2fef387ad
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060597"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="47739-103">删除 conversationMember</span><span class="sxs-lookup"><span data-stu-id="47739-103">Delete conversationMember</span></span>

<span data-ttu-id="47739-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47739-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="47739-105">从频道[中删除 conversationMember。](../resources/conversationmember.md) [](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="47739-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="47739-106">权限</span><span class="sxs-lookup"><span data-stu-id="47739-106">Permissions</span></span>

<span data-ttu-id="47739-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47739-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47739-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="47739-109">Permission Type</span></span>|<span data-ttu-id="47739-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47739-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="47739-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47739-111">Delegated (work or school account)</span></span>| <span data-ttu-id="47739-112">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47739-112">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="47739-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47739-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47739-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="47739-114">Not supported.</span></span>|
|<span data-ttu-id="47739-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="47739-115">Application</span></span>| <span data-ttu-id="47739-116">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47739-116">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47739-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47739-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="47739-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="47739-118">Request headers</span></span>

| <span data-ttu-id="47739-119">标头</span><span class="sxs-lookup"><span data-stu-id="47739-119">Header</span></span>       | <span data-ttu-id="47739-120">值</span><span class="sxs-lookup"><span data-stu-id="47739-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47739-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="47739-121">Authorization</span></span>  | <span data-ttu-id="47739-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="47739-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47739-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="47739-124">Request body</span></span>

<span data-ttu-id="47739-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="47739-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47739-126">响应</span><span class="sxs-lookup"><span data-stu-id="47739-126">Response</span></span>

<span data-ttu-id="47739-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="47739-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="47739-128">示例</span><span class="sxs-lookup"><span data-stu-id="47739-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="47739-129">请求</span><span class="sxs-lookup"><span data-stu-id="47739-129">Request</span></span>

<span data-ttu-id="47739-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="47739-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="47739-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="47739-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/V1.0/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="47739-132">C#</span><span class="sxs-lookup"><span data-stu-id="47739-132">C#</span></span>](#tab/csharp)

# <a name="javascript"></a>[<span data-ttu-id="47739-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47739-133">JavaScript</span></span>](#tab/javascript)

# <a name="objective-c"></a>[<span data-ttu-id="47739-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47739-134">Objective-C</span></span>](#tab/objc)

---

### <a name="response"></a><span data-ttu-id="47739-135">响应</span><span class="sxs-lookup"><span data-stu-id="47739-135">Response</span></span>

<span data-ttu-id="47739-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="47739-136">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

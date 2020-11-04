---
title: 删除 conversationMember
description: 从频道中删除 conversationMember。
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 05dd3377e5a3161a38d9db1d56de7bba7ccf9af4
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848323"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="f7ca8-103">删除 conversationMember</span><span class="sxs-lookup"><span data-stu-id="f7ca8-103">Delete conversationMember</span></span>

<span data-ttu-id="f7ca8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7ca8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7ca8-105">从[频道](../resources/channel.md)中删除[conversationMember](../resources/conversationmember.md) 。</span><span class="sxs-lookup"><span data-stu-id="f7ca8-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="f7ca8-106">权限</span><span class="sxs-lookup"><span data-stu-id="f7ca8-106">Permissions</span></span>

<span data-ttu-id="f7ca8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7ca8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7ca8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7ca8-109">Permission Type</span></span>|<span data-ttu-id="f7ca8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7ca8-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="f7ca8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7ca8-111">Delegated (work or school account)</span></span>| <span data-ttu-id="f7ca8-112">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7ca8-112">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="f7ca8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7ca8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7ca8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7ca8-114">Not supported.</span></span>|
|<span data-ttu-id="f7ca8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7ca8-115">Application</span></span>| <span data-ttu-id="f7ca8-116">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7ca8-116">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7ca8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7ca8-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f7ca8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7ca8-118">Request headers</span></span>

| <span data-ttu-id="f7ca8-119">标头</span><span class="sxs-lookup"><span data-stu-id="f7ca8-119">Header</span></span>       | <span data-ttu-id="f7ca8-120">值</span><span class="sxs-lookup"><span data-stu-id="f7ca8-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7ca8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7ca8-121">Authorization</span></span>  | <span data-ttu-id="f7ca8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7ca8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7ca8-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7ca8-124">Request body</span></span>

<span data-ttu-id="f7ca8-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7ca8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7ca8-126">响应</span><span class="sxs-lookup"><span data-stu-id="f7ca8-126">Response</span></span>

<span data-ttu-id="f7ca8-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f7ca8-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f7ca8-128">示例</span><span class="sxs-lookup"><span data-stu-id="f7ca8-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7ca8-129">请求</span><span class="sxs-lookup"><span data-stu-id="f7ca8-129">Request</span></span>

<span data-ttu-id="f7ca8-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7ca8-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7ca8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7ca8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/V1.0/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="f7ca8-132">C#</span><span class="sxs-lookup"><span data-stu-id="f7ca8-132">C#</span></span>](#tab/csharp)

# <a name="javascript"></a>[<span data-ttu-id="f7ca8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7ca8-133">JavaScript</span></span>](#tab/javascript)

# <a name="objective-c"></a>[<span data-ttu-id="f7ca8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7ca8-134">Objective-C</span></span>](#tab/objc)

---

### <a name="response"></a><span data-ttu-id="f7ca8-135">响应</span><span class="sxs-lookup"><span data-stu-id="f7ca8-135">Response</span></span>

<span data-ttu-id="f7ca8-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f7ca8-136">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

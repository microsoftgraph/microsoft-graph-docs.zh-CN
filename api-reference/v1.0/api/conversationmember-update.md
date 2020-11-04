---
title: 更新 conversationMember
description: 在团队或频道中更新 conversationMember 的角色。
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: efb4ed29e93dd2e73852a1589e233cefa7db8d11
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848311"
---
# <a name="update-conversationmember"></a><span data-ttu-id="455f2-103">更新 conversationMember</span><span class="sxs-lookup"><span data-stu-id="455f2-103">Update conversationMember</span></span>

<span data-ttu-id="455f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="455f2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="455f2-105">在[团队](../resources/team.md)或[频道](../resources/channel.md)中更新[conversationMember](../resources/conversationmember.md)的角色。</span><span class="sxs-lookup"><span data-stu-id="455f2-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [team](../resources/team.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="455f2-106">权限</span><span class="sxs-lookup"><span data-stu-id="455f2-106">Permissions</span></span>

<span data-ttu-id="455f2-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="455f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="455f2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="455f2-109">Permission Type</span></span>|<span data-ttu-id="455f2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="455f2-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="455f2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="455f2-111">Delegated (work or school account)</span></span>| <span data-ttu-id="455f2-112">在团队中： TeamMember</span><span class="sxs-lookup"><span data-stu-id="455f2-112">In teams: TeamMember.ReadWrite.All</span></span><br/><span data-ttu-id="455f2-113">在信道中： ChannelMember</span><span class="sxs-lookup"><span data-stu-id="455f2-113">In channels: ChannelMember.ReadWrite.All</span></span>  |
|<span data-ttu-id="455f2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="455f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="455f2-115">不支持</span><span class="sxs-lookup"><span data-stu-id="455f2-115">Not supported</span></span>|
|<span data-ttu-id="455f2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="455f2-116">Application</span></span>| <span data-ttu-id="455f2-117">在团队中： TeamMember</span><span class="sxs-lookup"><span data-stu-id="455f2-117">In teams: TeamMember.ReadWrite.All</span></span><br/><span data-ttu-id="455f2-118">在信道中： ChannelMember</span><span class="sxs-lookup"><span data-stu-id="455f2-118">In channels:  ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="455f2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="455f2-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="455f2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="455f2-120">Request headers</span></span>

| <span data-ttu-id="455f2-121">标头</span><span class="sxs-lookup"><span data-stu-id="455f2-121">Header</span></span>       | <span data-ttu-id="455f2-122">值</span><span class="sxs-lookup"><span data-stu-id="455f2-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="455f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="455f2-123">Authorization</span></span>  | <span data-ttu-id="455f2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="455f2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="455f2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="455f2-126">Request body</span></span>

<span data-ttu-id="455f2-127">在请求正文中，提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="455f2-127">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="455f2-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="455f2-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="455f2-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="455f2-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="455f2-130">属性</span><span class="sxs-lookup"><span data-stu-id="455f2-130">Property</span></span>   | <span data-ttu-id="455f2-131">类型</span><span class="sxs-lookup"><span data-stu-id="455f2-131">Type</span></span> |<span data-ttu-id="455f2-132">说明</span><span class="sxs-lookup"><span data-stu-id="455f2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="455f2-133">角色</span><span class="sxs-lookup"><span data-stu-id="455f2-133">roles</span></span>|<span data-ttu-id="455f2-134">string 集合</span><span class="sxs-lookup"><span data-stu-id="455f2-134">string collection</span></span>|<span data-ttu-id="455f2-135">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="455f2-135">The roles for that user.</span></span> <span data-ttu-id="455f2-136">必须为 "owner" 或空。</span><span class="sxs-lookup"><span data-stu-id="455f2-136">Must be "owner" or empty.</span></span> <span data-ttu-id="455f2-137">来宾用户必须始终拥有角色 "来宾"，并且无法更改。</span><span class="sxs-lookup"><span data-stu-id="455f2-137">Guest users must always have role "guest" and cannot change.</span></span> |

## <a name="response"></a><span data-ttu-id="455f2-138">响应</span><span class="sxs-lookup"><span data-stu-id="455f2-138">Response</span></span>

<span data-ttu-id="455f2-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="455f2-139">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="455f2-140">示例</span><span class="sxs-lookup"><span data-stu-id="455f2-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="455f2-141">请求</span><span class="sxs-lookup"><span data-stu-id="455f2-141">Request</span></span>

<span data-ttu-id="455f2-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="455f2-142">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_conversation_member"
} -->
```http
PATCH https://graph.microsoft.com/V1.0/teams/{id}/channels/{id}/members/{id}
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```

### <a name="response"></a><span data-ttu-id="455f2-143">响应</span><span class="sxs-lookup"><span data-stu-id="455f2-143">Response</span></span>

<span data-ttu-id="455f2-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="455f2-144">Here is an example of the response.</span></span>

><span data-ttu-id="455f2-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="455f2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 475

{
  "@odata.context": "https://graph.microsoft.com/V1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

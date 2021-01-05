---
title: '更新频道 '
description: 更新指定频道的属性。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a23916c9941afd17064e75add3e7c5ca5480fa54
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753455"
---
# <a name="update-channel"></a><span data-ttu-id="9face-103">更新频道 </span><span class="sxs-lookup"><span data-stu-id="9face-103">Update channel</span></span>

<span data-ttu-id="9face-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9face-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9face-105">更新指定频道 [的属性](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="9face-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9face-106">权限</span><span class="sxs-lookup"><span data-stu-id="9face-106">Permissions</span></span>

<span data-ttu-id="9face-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9face-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9face-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9face-109">Permission type</span></span>      | <span data-ttu-id="9face-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9face-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9face-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9face-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9face-112">ChannelSettings.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9face-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="9face-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9face-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9face-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9face-114">Not supported.</span></span>    |
|<span data-ttu-id="9face-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9face-115">Application</span></span> | <span data-ttu-id="9face-116">ChannelSettings.ReadWrite.Group\*、ChannelSettings.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9face-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="9face-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="9face-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="9face-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="9face-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9face-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="9face-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9face-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9face-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9face-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9face-121">Request headers</span></span>
| <span data-ttu-id="9face-122">标头</span><span class="sxs-lookup"><span data-stu-id="9face-122">Header</span></span>       | <span data-ttu-id="9face-123">值</span><span class="sxs-lookup"><span data-stu-id="9face-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9face-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9face-124">Authorization</span></span>  | <span data-ttu-id="9face-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9face-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9face-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9face-127">Content-Type</span></span>  | <span data-ttu-id="9face-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9face-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9face-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="9face-130">Request body</span></span>

<span data-ttu-id="9face-131">在请求正文中，提供 [channel](../resources/channel.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9face-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="9face-132">**注意：** 无法更新 `membershipType` 现有频道的值。</span><span class="sxs-lookup"><span data-stu-id="9face-132">**Note:** You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="9face-133">响应</span><span class="sxs-lookup"><span data-stu-id="9face-133">Response</span></span>

<span data-ttu-id="9face-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9face-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9face-135">示例</span><span class="sxs-lookup"><span data-stu-id="9face-135">Example</span></span>

### <a name="example-1-update-channel"></a><span data-ttu-id="9face-136">示例 1：更新频道</span><span class="sxs-lookup"><span data-stu-id="9face-136">Example 1: Update channel</span></span>

#### <a name="request"></a><span data-ttu-id="9face-137">请求</span><span class="sxs-lookup"><span data-stu-id="9face-137">Request</span></span>

<span data-ttu-id="9face-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9face-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9face-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="9face-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="9face-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9face-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9face-141">响应</span><span class="sxs-lookup"><span data-stu-id="9face-141">Response</span></span>

<span data-ttu-id="9face-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9face-142">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-channel-with-moderation-settings"></a><span data-ttu-id="9face-143">示例 2：使用审核设置更新频道</span><span class="sxs-lookup"><span data-stu-id="9face-143">Example 2: Update channel with moderation settings</span></span>

#### <a name="request"></a><span data-ttu-id="9face-144">请求</span><span class="sxs-lookup"><span data-stu-id="9face-144">Request</span></span>

<span data-ttu-id="9face-145">以下示例显示更新频道 [的审核设置](../resources/channelmoderationsettings.md) 的请求。</span><span class="sxs-lookup"><span data-stu-id="9face-145">The following example shows a request to update the [moderation settings](../resources/channelmoderationsettings.md) of a channel.</span></span> <span data-ttu-id="9face-146">此操作只能由团队所有者执行。</span><span class="sxs-lookup"><span data-stu-id="9face-146">This operation can only be performed by a team owner.</span></span>

<!-- {
  "blockType": "request",
  "name": "patch_channel_with_moderationSettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/{team-id}/channels/{channel-id}
Content-type: application/json

{
    "displayName": "UpdateChannelModeration",
    "description": "Update channel moderation.",
    "moderationSettings": {
        "userNewMessageRestriction": "moderators",
        "replyRestriction": "everyone",
        "allowNewMessageFromBots": true,
        "allowNewMessageFromConnectors": true
    }
}
```


#### <a name="response"></a><span data-ttu-id="9face-147">响应</span><span class="sxs-lookup"><span data-stu-id="9face-147">Response</span></span>

<span data-ttu-id="9face-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9face-148">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



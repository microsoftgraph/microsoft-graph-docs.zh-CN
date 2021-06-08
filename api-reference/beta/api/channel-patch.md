---
title: '更新频道 '
description: 更新指定频道的属性。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8527ae77c6198aea615aff8add5a569dc563bafa
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786213"
---
# <a name="update-channel"></a><span data-ttu-id="90b7e-103">更新频道 </span><span class="sxs-lookup"><span data-stu-id="90b7e-103">Update channel</span></span>

<span data-ttu-id="90b7e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90b7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90b7e-105">更新指定频道 [的属性](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="90b7e-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="90b7e-106">权限</span><span class="sxs-lookup"><span data-stu-id="90b7e-106">Permissions</span></span>

<span data-ttu-id="90b7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90b7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90b7e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="90b7e-109">Permission type</span></span>      | <span data-ttu-id="90b7e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90b7e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90b7e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90b7e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="90b7e-112">ChannelSettings.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90b7e-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="90b7e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90b7e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90b7e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="90b7e-114">Not supported.</span></span>    |
|<span data-ttu-id="90b7e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="90b7e-115">Application</span></span> | <span data-ttu-id="90b7e-116">ChannelSettings.ReadWrite.Group\*、ChannelSettings.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90b7e-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="90b7e-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="90b7e-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="90b7e-p102">**注意**：此 API 支持管理员权限。全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="90b7e-p102">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="90b7e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90b7e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{team-id}/channels/{channel-id}
```
## <a name="request-headers"></a><span data-ttu-id="90b7e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="90b7e-121">Request headers</span></span>
| <span data-ttu-id="90b7e-122">标头</span><span class="sxs-lookup"><span data-stu-id="90b7e-122">Header</span></span>       | <span data-ttu-id="90b7e-123">值</span><span class="sxs-lookup"><span data-stu-id="90b7e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="90b7e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="90b7e-124">Authorization</span></span>  | <span data-ttu-id="90b7e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90b7e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="90b7e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="90b7e-127">Content-Type</span></span>  | <span data-ttu-id="90b7e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="90b7e-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="90b7e-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="90b7e-130">Request body</span></span>

<span data-ttu-id="90b7e-131">在请求正文中，提供 [channel](../resources/channel.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90b7e-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="90b7e-132">**注意：** 无法更新 `membershipType` 现有通道的值。</span><span class="sxs-lookup"><span data-stu-id="90b7e-132">**Note:** You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="90b7e-133">响应</span><span class="sxs-lookup"><span data-stu-id="90b7e-133">Response</span></span>

<span data-ttu-id="90b7e-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="90b7e-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="90b7e-135">示例</span><span class="sxs-lookup"><span data-stu-id="90b7e-135">Example</span></span>

### <a name="example-1-update-channel"></a><span data-ttu-id="90b7e-136">示例 1：更新频道</span><span class="sxs-lookup"><span data-stu-id="90b7e-136">Example 1: Update channel</span></span>

#### <a name="request"></a><span data-ttu-id="90b7e-137">请求</span><span class="sxs-lookup"><span data-stu-id="90b7e-137">Request</span></span>

<span data-ttu-id="90b7e-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90b7e-138">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
```


#### <a name="response"></a><span data-ttu-id="90b7e-139">响应</span><span class="sxs-lookup"><span data-stu-id="90b7e-139">Response</span></span>

<span data-ttu-id="90b7e-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="90b7e-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-channel-with-moderation-settings"></a><span data-ttu-id="90b7e-141">示例 2：使用审核设置更新频道</span><span class="sxs-lookup"><span data-stu-id="90b7e-141">Example 2: Update channel with moderation settings</span></span>

#### <a name="request"></a><span data-ttu-id="90b7e-142">请求</span><span class="sxs-lookup"><span data-stu-id="90b7e-142">Request</span></span>

<span data-ttu-id="90b7e-143">以下示例显示更新频道 [的审核设置](../resources/channelmoderationsettings.md) 的请求。</span><span class="sxs-lookup"><span data-stu-id="90b7e-143">The following example shows a request to update the [moderation settings](../resources/channelmoderationsettings.md) of a channel.</span></span> <span data-ttu-id="90b7e-144">此操作只能由团队所有者执行。</span><span class="sxs-lookup"><span data-stu-id="90b7e-144">This operation can only be performed by a team owner.</span></span>



# <a name="http"></a>[<span data-ttu-id="90b7e-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="90b7e-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel_with_moderationSettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
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
# <a name="c"></a>[<span data-ttu-id="90b7e-146">C#</span><span class="sxs-lookup"><span data-stu-id="90b7e-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-channel-with-moderationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90b7e-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90b7e-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-channel-with-moderationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90b7e-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90b7e-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-with-moderationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90b7e-149">Java</span><span class="sxs-lookup"><span data-stu-id="90b7e-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-channel-with-moderationsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a><span data-ttu-id="90b7e-150">响应</span><span class="sxs-lookup"><span data-stu-id="90b7e-150">Response</span></span>

<span data-ttu-id="90b7e-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="90b7e-151">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response"
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



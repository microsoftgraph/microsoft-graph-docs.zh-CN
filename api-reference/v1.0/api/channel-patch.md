---
title: 修补程序通道
description: 更新指定频道的属性。
author: anandjo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4c611ea955c82be94f5e0220fe0632d2c5791fc8
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51506868"
---
# <a name="patch-channel"></a><span data-ttu-id="cf3d4-103">修补程序通道</span><span class="sxs-lookup"><span data-stu-id="cf3d4-103">Patch channel</span></span>

<span data-ttu-id="cf3d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf3d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cf3d4-105">更新指定频道 [的属性](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="cf3d4-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf3d4-106">权限</span><span class="sxs-lookup"><span data-stu-id="cf3d4-106">Permissions</span></span>

<span data-ttu-id="cf3d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf3d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf3d4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf3d4-109">Permission type</span></span>      | <span data-ttu-id="cf3d4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf3d4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf3d4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf3d4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cf3d4-112">ChannelSettings.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf3d4-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="cf3d4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf3d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf3d4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf3d4-114">Not supported.</span></span>    |
|<span data-ttu-id="cf3d4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf3d4-115">Application</span></span> | <span data-ttu-id="cf3d4-116">ChannelSettings.ReadWrite.Group\*、ChannelSettings.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf3d4-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="cf3d4-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="cf3d4-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="cf3d4-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="cf3d4-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cf3d4-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="cf3d4-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cf3d4-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf3d4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{team-id}/channels/{channel-id}
```

## <a name="request-headers"></a><span data-ttu-id="cf3d4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf3d4-121">Request headers</span></span>
| <span data-ttu-id="cf3d4-122">标头</span><span class="sxs-lookup"><span data-stu-id="cf3d4-122">Header</span></span>       | <span data-ttu-id="cf3d4-123">值</span><span class="sxs-lookup"><span data-stu-id="cf3d4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cf3d4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf3d4-124">Authorization</span></span>  | <span data-ttu-id="cf3d4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf3d4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cf3d4-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cf3d4-127">Content-Type</span></span>  | <span data-ttu-id="cf3d4-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cf3d4-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf3d4-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf3d4-130">Request body</span></span>

<span data-ttu-id="cf3d4-131">在请求正文中，提供 [channel](../resources/channel.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf3d4-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="cf3d4-132">**注意：** 无法更新 `membershipType` 现有通道的值。</span><span class="sxs-lookup"><span data-stu-id="cf3d4-132">**Note:** You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="cf3d4-133">响应</span><span class="sxs-lookup"><span data-stu-id="cf3d4-133">Response</span></span>

<span data-ttu-id="cf3d4-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cf3d4-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cf3d4-135">示例</span><span class="sxs-lookup"><span data-stu-id="cf3d4-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf3d4-136">请求</span><span class="sxs-lookup"><span data-stu-id="cf3d4-136">Request</span></span>

<span data-ttu-id="cf3d4-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf3d4-137">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cf3d4-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf3d4-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
```
# <a name="objective-c"></a>[<span data-ttu-id="cf3d4-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf3d4-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cf3d4-140">响应</span><span class="sxs-lookup"><span data-stu-id="cf3d4-140">Response</span></span>

<span data-ttu-id="cf3d4-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cf3d4-141">Here is an example of the response.</span></span> 
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

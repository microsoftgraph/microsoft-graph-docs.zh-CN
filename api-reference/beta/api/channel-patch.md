---
title: 修补程序通道
description: 更新指定通道的属性。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 208fba1dff20fb4b8ac6979013378b9f8ac40171
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987104"
---
# <a name="patch-channel"></a><span data-ttu-id="18528-103">修补程序通道</span><span class="sxs-lookup"><span data-stu-id="18528-103">Patch channel</span></span>

<span data-ttu-id="18528-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18528-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18528-105">更新指定 [通道](../resources/channel.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="18528-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="18528-106">权限</span><span class="sxs-lookup"><span data-stu-id="18528-106">Permissions</span></span>

<span data-ttu-id="18528-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18528-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18528-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="18528-109">Permission type</span></span>      | <span data-ttu-id="18528-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18528-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18528-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18528-111">Delegated (work or school account)</span></span> | <span data-ttu-id="18528-112">ChannelSettings、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="18528-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="18528-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18528-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18528-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="18528-114">Not supported.</span></span>    |
|<span data-ttu-id="18528-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="18528-115">Application</span></span> | <span data-ttu-id="18528-116">ChannelSettings \*、ChannelSettings、all、ReadWrite、all、all、All、All</span><span class="sxs-lookup"><span data-stu-id="18528-116">ChannelSettings.Edit.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="18528-117">**注意**：标有 \* 的权限用于[特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="18528-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="18528-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="18528-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="18528-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="18528-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="18528-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18528-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="18528-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="18528-121">Request headers</span></span>
| <span data-ttu-id="18528-122">标头</span><span class="sxs-lookup"><span data-stu-id="18528-122">Header</span></span>       | <span data-ttu-id="18528-123">值</span><span class="sxs-lookup"><span data-stu-id="18528-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18528-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="18528-124">Authorization</span></span>  | <span data-ttu-id="18528-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18528-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="18528-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18528-127">Content-Type</span></span>  | <span data-ttu-id="18528-128">application/json</span><span class="sxs-lookup"><span data-stu-id="18528-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18528-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="18528-129">Request body</span></span>

<span data-ttu-id="18528-130">在请求正文中，提供 [channel](../resources/channel.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18528-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="18528-131">注意：不能更新 `membershipType` 现有频道的值。</span><span class="sxs-lookup"><span data-stu-id="18528-131">Note: You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="18528-132">响应</span><span class="sxs-lookup"><span data-stu-id="18528-132">Response</span></span>

<span data-ttu-id="18528-133">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="18528-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="18528-134">示例</span><span class="sxs-lookup"><span data-stu-id="18528-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="18528-135">请求</span><span class="sxs-lookup"><span data-stu-id="18528-135">Request</span></span>

<span data-ttu-id="18528-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18528-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18528-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="18528-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="18528-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18528-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="18528-139">响应</span><span class="sxs-lookup"><span data-stu-id="18528-139">Response</span></span>

<span data-ttu-id="18528-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18528-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



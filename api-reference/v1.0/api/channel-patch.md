---
title: 修补程序通道
description: 更新指定通道的属性。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3b46315ce93574a778e56fba9f924c2959413d64
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863920"
---
# <a name="patch-channel"></a><span data-ttu-id="7e13a-103">修补程序通道</span><span class="sxs-lookup"><span data-stu-id="7e13a-103">Patch channel</span></span>

<span data-ttu-id="7e13a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e13a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e13a-105">更新指定[通道](../resources/channel.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="7e13a-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e13a-106">权限</span><span class="sxs-lookup"><span data-stu-id="7e13a-106">Permissions</span></span>

<span data-ttu-id="7e13a-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7e13a-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7e13a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e13a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e13a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e13a-109">Permission type</span></span>      | <span data-ttu-id="7e13a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e13a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e13a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e13a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7e13a-112">ChannelSettings、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="7e13a-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="7e13a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e13a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e13a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e13a-114">Not supported.</span></span>    |
|<span data-ttu-id="7e13a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e13a-115">Application</span></span> | <span data-ttu-id="7e13a-116">ChannelSettings、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="7e13a-116">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="7e13a-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="7e13a-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="7e13a-118">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="7e13a-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="7e13a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e13a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7e13a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e13a-120">Request headers</span></span>

| <span data-ttu-id="7e13a-121">标头</span><span class="sxs-lookup"><span data-stu-id="7e13a-121">Header</span></span>       | <span data-ttu-id="7e13a-122">值</span><span class="sxs-lookup"><span data-stu-id="7e13a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7e13a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e13a-123">Authorization</span></span>  | <span data-ttu-id="7e13a-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="7e13a-124">Bearer {token}.</span></span> <span data-ttu-id="7e13a-125">Required.</span><span class="sxs-lookup"><span data-stu-id="7e13a-125">Required.</span></span>  |
| <span data-ttu-id="7e13a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e13a-126">Content-Type</span></span>  | <span data-ttu-id="7e13a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7e13a-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7e13a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e13a-128">Request body</span></span>

<span data-ttu-id="7e13a-129">在请求正文中，提供 [channel](../resources/channel.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e13a-129">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7e13a-130">响应</span><span class="sxs-lookup"><span data-stu-id="7e13a-130">Response</span></span>

<span data-ttu-id="7e13a-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7e13a-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7e13a-132">示例</span><span class="sxs-lookup"><span data-stu-id="7e13a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e13a-133">请求</span><span class="sxs-lookup"><span data-stu-id="7e13a-133">Request</span></span>

<span data-ttu-id="7e13a-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7e13a-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e13a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e13a-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="7e13a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e13a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="7e13a-137">响应</span><span class="sxs-lookup"><span data-stu-id="7e13a-137">Response</span></span>

<span data-ttu-id="7e13a-138">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="7e13a-138">Here is an example of the response.</span></span> <span data-ttu-id="7e13a-139">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="7e13a-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7e13a-140">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="7e13a-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 204 No Content
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

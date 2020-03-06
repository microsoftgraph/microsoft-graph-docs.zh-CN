---
title: 修补程序通道
description: 更新指定通道的属性。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 68265b319fd567097b72c9eaad82275fd3faefab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518600"
---
# <a name="patch-channel"></a><span data-ttu-id="e0ef6-103">修补程序通道</span><span class="sxs-lookup"><span data-stu-id="e0ef6-103">Patch channel</span></span>

<span data-ttu-id="e0ef6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0ef6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e0ef6-105">更新指定[通道](../resources/channel.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="e0ef6-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e0ef6-106">权限</span><span class="sxs-lookup"><span data-stu-id="e0ef6-106">Permissions</span></span>

<span data-ttu-id="e0ef6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0ef6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0ef6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0ef6-109">Permission type</span></span>      | <span data-ttu-id="e0ef6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0ef6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0ef6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0ef6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e0ef6-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0ef6-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e0ef6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0ef6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0ef6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0ef6-114">Not supported.</span></span>    |
|<span data-ttu-id="e0ef6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0ef6-115">Application</span></span> | <span data-ttu-id="e0ef6-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0ef6-116">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="e0ef6-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="e0ef6-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e0ef6-118">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="e0ef6-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e0ef6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0ef6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e0ef6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0ef6-120">Request headers</span></span>

| <span data-ttu-id="e0ef6-121">标头</span><span class="sxs-lookup"><span data-stu-id="e0ef6-121">Header</span></span>       | <span data-ttu-id="e0ef6-122">值</span><span class="sxs-lookup"><span data-stu-id="e0ef6-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0ef6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0ef6-123">Authorization</span></span>  | <span data-ttu-id="e0ef6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0ef6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e0ef6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0ef6-126">Content-Type</span></span>  | <span data-ttu-id="e0ef6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e0ef6-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0ef6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0ef6-128">Request body</span></span>

<span data-ttu-id="e0ef6-129">在请求正文中，提供 [channel](../resources/channel.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0ef6-129">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e0ef6-130">响应</span><span class="sxs-lookup"><span data-stu-id="e0ef6-130">Response</span></span>

<span data-ttu-id="e0ef6-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e0ef6-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e0ef6-132">示例</span><span class="sxs-lookup"><span data-stu-id="e0ef6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0ef6-133">请求</span><span class="sxs-lookup"><span data-stu-id="e0ef6-133">Request</span></span>

<span data-ttu-id="e0ef6-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0ef6-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0ef6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0ef6-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="e0ef6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0ef6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e0ef6-137">响应</span><span class="sxs-lookup"><span data-stu-id="e0ef6-137">Response</span></span>

<span data-ttu-id="e0ef6-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e0ef6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
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

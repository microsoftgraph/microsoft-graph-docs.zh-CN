---
title: 修补程序通道
description: 更新指定的频道的属性。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 73d777999d6112de44cffc6fb8e9a4cd36ee093c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832833"
---
# <a name="patch-channel"></a><span data-ttu-id="531d7-103">修补程序通道</span><span class="sxs-lookup"><span data-stu-id="531d7-103">Patch channel</span></span>



<span data-ttu-id="531d7-104">更新指定的[频道](../resources/channel.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="531d7-104">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="531d7-105">**注意**： 没有应用程序权限和此 API 的已知的问题。</span><span class="sxs-lookup"><span data-stu-id="531d7-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="531d7-106">有关详细信息，请参阅[已知问题列表](/graph/known-issues#application-permissions)。</span><span class="sxs-lookup"><span data-stu-id="531d7-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="531d7-107">权限</span><span class="sxs-lookup"><span data-stu-id="531d7-107">Permissions</span></span>
<span data-ttu-id="531d7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="531d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="531d7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="531d7-110">Permission type</span></span>      | <span data-ttu-id="531d7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="531d7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="531d7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="531d7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="531d7-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="531d7-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="531d7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="531d7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="531d7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="531d7-115">Not supported.</span></span>    |
|<span data-ttu-id="531d7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="531d7-116">Application</span></span> | <span data-ttu-id="531d7-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="531d7-117">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="531d7-118">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="531d7-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="531d7-119">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="531d7-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="531d7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="531d7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="531d7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="531d7-121">Request headers</span></span>
| <span data-ttu-id="531d7-122">标头</span><span class="sxs-lookup"><span data-stu-id="531d7-122">Header</span></span>       | <span data-ttu-id="531d7-123">值</span><span class="sxs-lookup"><span data-stu-id="531d7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="531d7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="531d7-124">Authorization</span></span>  | <span data-ttu-id="531d7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="531d7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="531d7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="531d7-127">Content-Type</span></span>  | <span data-ttu-id="531d7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="531d7-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="531d7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="531d7-129">Request body</span></span>
<span data-ttu-id="531d7-130">在请求正文中，提供[信道](../resources/channel.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="531d7-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="531d7-131">响应</span><span class="sxs-lookup"><span data-stu-id="531d7-131">Response</span></span>

<span data-ttu-id="531d7-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="531d7-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="531d7-133">示例</span><span class="sxs-lookup"><span data-stu-id="531d7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="531d7-134">请求</span><span class="sxs-lookup"><span data-stu-id="531d7-134">Request</span></span>
<span data-ttu-id="531d7-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="531d7-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="531d7-136">响应</span><span class="sxs-lookup"><span data-stu-id="531d7-136">Response</span></span>
<span data-ttu-id="531d7-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="531d7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->

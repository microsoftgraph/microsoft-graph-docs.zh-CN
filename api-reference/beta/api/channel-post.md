---
title: 创建通道
description: 在 Microsoft 团队，在请求正文中的规定创建新的通道。
localization_priority: Normal
ms.openlocfilehash: f7192c177d79e48a0a9e55c9edc5dbb394539928
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875045"
---
# <a name="create-channel"></a><span data-ttu-id="4aa28-103">创建通道</span><span class="sxs-lookup"><span data-stu-id="4aa28-103">Create Channel</span></span>

> <span data-ttu-id="4aa28-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4aa28-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4aa28-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4aa28-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4aa28-106">在 Microsoft 团队，在请求正文中的规定创建新的[通道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="4aa28-106">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="4aa28-107">**注意**： 没有应用程序权限和此 API 的已知的问题。</span><span class="sxs-lookup"><span data-stu-id="4aa28-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="4aa28-108">有关详细信息，请参阅[已知问题列表](/graph/known-issues#application-permissions)。</span><span class="sxs-lookup"><span data-stu-id="4aa28-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="4aa28-109">权限</span><span class="sxs-lookup"><span data-stu-id="4aa28-109">Permissions</span></span>
<span data-ttu-id="4aa28-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4aa28-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4aa28-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4aa28-112">Permission type</span></span>      | <span data-ttu-id="4aa28-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4aa28-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4aa28-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4aa28-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4aa28-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4aa28-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4aa28-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4aa28-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4aa28-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4aa28-117">Not supported.</span></span>    |
|<span data-ttu-id="4aa28-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4aa28-118">Application</span></span> | <span data-ttu-id="4aa28-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4aa28-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="4aa28-120">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="4aa28-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4aa28-121">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="4aa28-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4aa28-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4aa28-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="4aa28-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="4aa28-123">Request headers</span></span>
| <span data-ttu-id="4aa28-124">标头</span><span class="sxs-lookup"><span data-stu-id="4aa28-124">Header</span></span>       | <span data-ttu-id="4aa28-125">值</span><span class="sxs-lookup"><span data-stu-id="4aa28-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4aa28-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aa28-126">Authorization</span></span>  | <span data-ttu-id="4aa28-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4aa28-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4aa28-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4aa28-129">Content-Type</span></span>  | <span data-ttu-id="4aa28-130">application/json</span><span class="sxs-lookup"><span data-stu-id="4aa28-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4aa28-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="4aa28-131">Request body</span></span>
<span data-ttu-id="4aa28-132">在请求正文中，提供[信道](../resources/channel.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4aa28-132">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4aa28-133">响应</span><span class="sxs-lookup"><span data-stu-id="4aa28-133">Response</span></span>

<span data-ttu-id="4aa28-134">如果成功，此方法返回`201 Created`响应正文中的响应代码和[频道](../resources/channel.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4aa28-134">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4aa28-135">示例</span><span class="sxs-lookup"><span data-stu-id="4aa28-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4aa28-136">请求</span><span class="sxs-lookup"><span data-stu-id="4aa28-136">Request</span></span>
<span data-ttu-id="4aa28-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4aa28-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
##### <a name="response"></a><span data-ttu-id="4aa28-138">响应</span><span class="sxs-lookup"><span data-stu-id="4aa28-138">Response</span></span>
<span data-ttu-id="4aa28-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4aa28-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

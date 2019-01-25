---
title: 呼叫： changeScreenSharingRole
description: 启动和停止共享的调用中的屏幕。 此 API 用于允许应用程序共享屏幕内容与呼叫或会议的参与者。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f0bdd9a4c8e900d9a1ec5f7801fa959ebdaae1e1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514731"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="a91de-104">呼叫： changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="a91de-104">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a91de-105">启动和停止共享的调用中的屏幕。</span><span class="sxs-lookup"><span data-stu-id="a91de-105">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="a91de-106">此 API 用于允许应用程序共享屏幕内容与呼叫或会议的参与者。</span><span class="sxs-lookup"><span data-stu-id="a91de-106">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="a91de-107">权限</span><span class="sxs-lookup"><span data-stu-id="a91de-107">Permissions</span></span>
<span data-ttu-id="a91de-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a91de-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a91de-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a91de-110">Permission type</span></span>                        | <span data-ttu-id="a91de-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a91de-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a91de-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a91de-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a91de-113">不支持</span><span class="sxs-lookup"><span data-stu-id="a91de-113">Not Supported</span></span>                               |
| <span data-ttu-id="a91de-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a91de-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a91de-115">不支持</span><span class="sxs-lookup"><span data-stu-id="a91de-115">Not Supported</span></span>                               |
| <span data-ttu-id="a91de-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a91de-116">Application</span></span>                            | <span data-ttu-id="a91de-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="a91de-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="a91de-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a91de-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="a91de-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a91de-119">Request headers</span></span>
| <span data-ttu-id="a91de-120">名称</span><span class="sxs-lookup"><span data-stu-id="a91de-120">Name</span></span>          | <span data-ttu-id="a91de-121">说明</span><span class="sxs-lookup"><span data-stu-id="a91de-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a91de-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a91de-122">Authorization</span></span> | <span data-ttu-id="a91de-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a91de-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a91de-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a91de-125">Request body</span></span>
<span data-ttu-id="a91de-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a91de-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a91de-127">参数</span><span class="sxs-lookup"><span data-stu-id="a91de-127">Parameter</span></span>      | <span data-ttu-id="a91de-128">类型</span><span class="sxs-lookup"><span data-stu-id="a91de-128">Type</span></span>    |<span data-ttu-id="a91de-129">说明</span><span class="sxs-lookup"><span data-stu-id="a91de-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a91de-130">role</span><span class="sxs-lookup"><span data-stu-id="a91de-130">role</span></span>|<span data-ttu-id="a91de-131">String</span><span class="sxs-lookup"><span data-stu-id="a91de-131">String</span></span>|<span data-ttu-id="a91de-132">可能的值为: 查看、 共享</span><span class="sxs-lookup"><span data-stu-id="a91de-132">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="a91de-133">响应</span><span class="sxs-lookup"><span data-stu-id="a91de-133">Response</span></span>
<span data-ttu-id="a91de-134">返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="a91de-134">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a91de-135">示例</span><span class="sxs-lookup"><span data-stu-id="a91de-135">Example</span></span>
<span data-ttu-id="a91de-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a91de-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a91de-137">请求</span><span class="sxs-lookup"><span data-stu-id="a91de-137">Request</span></span>
<span data-ttu-id="a91de-138">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="a91de-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```

##### <a name="response"></a><span data-ttu-id="a91de-139">响应</span><span class="sxs-lookup"><span data-stu-id="a91de-139">Response</span></span>
<span data-ttu-id="a91de-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a91de-140">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-changescreensharingrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: '调用: changeScreenSharingRole'
description: 在呼叫中开始和停止共享屏幕。 此 API 用于允许应用程序与呼叫或会议的参与者共享屏幕内容。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f0bdd9a4c8e900d9a1ec5f7801fa959ebdaae1e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461273"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="3f89c-104">调用: changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="3f89c-104">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f89c-105">在呼叫中开始和停止共享屏幕。</span><span class="sxs-lookup"><span data-stu-id="3f89c-105">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="3f89c-106">此 API 用于允许应用程序与呼叫或会议的参与者共享屏幕内容。</span><span class="sxs-lookup"><span data-stu-id="3f89c-106">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f89c-107">权限</span><span class="sxs-lookup"><span data-stu-id="3f89c-107">Permissions</span></span>
<span data-ttu-id="3f89c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f89c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3f89c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f89c-110">Permission type</span></span>                        | <span data-ttu-id="3f89c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f89c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3f89c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f89c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f89c-113">不支持</span><span class="sxs-lookup"><span data-stu-id="3f89c-113">Not Supported</span></span>                               |
| <span data-ttu-id="3f89c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f89c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f89c-115">不支持</span><span class="sxs-lookup"><span data-stu-id="3f89c-115">Not Supported</span></span>                               |
| <span data-ttu-id="3f89c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f89c-116">Application</span></span>                            | <span data-ttu-id="3f89c-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="3f89c-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="3f89c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f89c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="3f89c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f89c-119">Request headers</span></span>
| <span data-ttu-id="3f89c-120">名称</span><span class="sxs-lookup"><span data-stu-id="3f89c-120">Name</span></span>          | <span data-ttu-id="3f89c-121">说明</span><span class="sxs-lookup"><span data-stu-id="3f89c-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3f89c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f89c-122">Authorization</span></span> | <span data-ttu-id="3f89c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3f89c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f89c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f89c-125">Request body</span></span>
<span data-ttu-id="3f89c-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3f89c-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3f89c-127">参数</span><span class="sxs-lookup"><span data-stu-id="3f89c-127">Parameter</span></span>      | <span data-ttu-id="3f89c-128">类型</span><span class="sxs-lookup"><span data-stu-id="3f89c-128">Type</span></span>    |<span data-ttu-id="3f89c-129">说明</span><span class="sxs-lookup"><span data-stu-id="3f89c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f89c-130">role</span><span class="sxs-lookup"><span data-stu-id="3f89c-130">role</span></span>|<span data-ttu-id="3f89c-131">字符串</span><span class="sxs-lookup"><span data-stu-id="3f89c-131">String</span></span>|<span data-ttu-id="3f89c-132">可能的值为: "查看器"、"共享资源"</span><span class="sxs-lookup"><span data-stu-id="3f89c-132">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="3f89c-133">响应</span><span class="sxs-lookup"><span data-stu-id="3f89c-133">Response</span></span>
<span data-ttu-id="3f89c-134">返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="3f89c-134">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3f89c-135">示例</span><span class="sxs-lookup"><span data-stu-id="3f89c-135">Example</span></span>
<span data-ttu-id="3f89c-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="3f89c-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3f89c-137">请求</span><span class="sxs-lookup"><span data-stu-id="3f89c-137">Request</span></span>
<span data-ttu-id="3f89c-138">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f89c-138">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="3f89c-139">响应</span><span class="sxs-lookup"><span data-stu-id="3f89c-139">Response</span></span>
<span data-ttu-id="3f89c-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3f89c-140">Here is an example of the response.</span></span> 

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

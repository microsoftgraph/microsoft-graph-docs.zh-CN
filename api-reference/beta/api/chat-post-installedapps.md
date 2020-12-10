---
title: 将应用添加到聊天
description: 将应用安装到聊天。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ce4e7c8bee2535840b2d0f3d6fb234fb38ffbaf2
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607488"
---
# <a name="add-app-to-chat"></a><span data-ttu-id="674ab-103">将应用添加到聊天</span><span class="sxs-lookup"><span data-stu-id="674ab-103">Add app to chat</span></span>

<span data-ttu-id="674ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="674ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="674ab-105">将 [teamsApp](../resources/teamsapp.md) 安装到指定的[聊天](../resources/chat.md)中。</span><span class="sxs-lookup"><span data-stu-id="674ab-105">Install a [teamsApp](../resources/teamsapp.md) to the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="674ab-106">权限</span><span class="sxs-lookup"><span data-stu-id="674ab-106">Permissions</span></span>

<span data-ttu-id="674ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="674ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="674ab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="674ab-109">Permission type</span></span>      | <span data-ttu-id="674ab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="674ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="674ab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="674ab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="674ab-112">TeamsAppInstallation.ReadWriteSelfForChat、TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="674ab-112">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="674ab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="674ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="674ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="674ab-114">Not supported.</span></span>    |
|<span data-ttu-id="674ab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="674ab-115">Application</span></span> | <span data-ttu-id="674ab-116">TeamsAppInstallation.ReadWriteSelfForChat.All、TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="674ab-116">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="674ab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="674ab-117">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
POST /chats/{chat-id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="674ab-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="674ab-118">Request headers</span></span>

| <span data-ttu-id="674ab-119">标头</span><span class="sxs-lookup"><span data-stu-id="674ab-119">Header</span></span>       | <span data-ttu-id="674ab-120">值</span><span class="sxs-lookup"><span data-stu-id="674ab-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="674ab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="674ab-121">Authorization</span></span>  | <span data-ttu-id="674ab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="674ab-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="674ab-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="674ab-124">Content-Type</span></span>  | <span data-ttu-id="674ab-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="674ab-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="674ab-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="674ab-127">Request body</span></span>

<span data-ttu-id="674ab-128">请求正文应包含目录应用的生成应用 ID。</span><span class="sxs-lookup"><span data-stu-id="674ab-128">The request body should contain the catalog app's generated app ID.</span></span> <span data-ttu-id="674ab-129">有关详细信息，请参阅 [teamsApp 属性](../resources/teamsapp.md#properties)。</span><span class="sxs-lookup"><span data-stu-id="674ab-129">For details, see [teamsApp properties](../resources/teamsapp.md#properties).</span></span>

## <a name="response"></a><span data-ttu-id="674ab-130">响应</span><span class="sxs-lookup"><span data-stu-id="674ab-130">Response</span></span>

<span data-ttu-id="674ab-131">如果成功，此方法返回 `201 Created` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="674ab-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="674ab-132">示例</span><span class="sxs-lookup"><span data-stu-id="674ab-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="674ab-133">请求</span><span class="sxs-lookup"><span data-stu-id="674ab-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "add_app_in_chat"
}-->

```http
POST https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps
Content-Type: application/json

{
"teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a><span data-ttu-id="674ab-134">响应</span><span class="sxs-lookup"><span data-stu-id="674ab-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation"
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat add installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

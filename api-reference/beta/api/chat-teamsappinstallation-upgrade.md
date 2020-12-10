---
title: teamsAppInstallation：升级
description: 更新聊天中安装的应用程序，并使其与租户应用目录中提供的当前版本保持同步。
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f3c68d21a5af7cb724bf0990e3af216ce54a28b4
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607487"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="b59d8-103">teamsAppInstallation：升级</span><span class="sxs-lookup"><span data-stu-id="b59d8-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="b59d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b59d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b59d8-105">升级[聊天](../resources/chat.md)中的[应用安装](../resources/teamsappinstallation.md)。</span><span class="sxs-lookup"><span data-stu-id="b59d8-105">Upgrade an [app installation](../resources/teamsappinstallation.md) within a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b59d8-106">权限</span><span class="sxs-lookup"><span data-stu-id="b59d8-106">Permissions</span></span>

<span data-ttu-id="b59d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b59d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b59d8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b59d8-109">Permission type</span></span>      | <span data-ttu-id="b59d8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b59d8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b59d8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b59d8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b59d8-112">TeamsAppInstallation.ReadWriteSelfForChat、TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="b59d8-112">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="b59d8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b59d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b59d8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b59d8-114">Not supported.</span></span>   |
|<span data-ttu-id="b59d8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b59d8-115">Application</span></span> | <span data-ttu-id="b59d8-116">TeamsAppInstallation.ReadWriteSelfForChat.All、TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="b59d8-116">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b59d8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b59d8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /chats/{chat-id}/installedApps/{app-installation-id}/upgrade
```

## <a name="response"></a><span data-ttu-id="b59d8-118">响应</span><span class="sxs-lookup"><span data-stu-id="b59d8-118">Response</span></span>

<span data-ttu-id="b59d8-119">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b59d8-119">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b59d8-120">示例</span><span class="sxs-lookup"><span data-stu-id="b59d8-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="b59d8-121">请求</span><span class="sxs-lookup"><span data-stu-id="b59d8-121">Request</span></span>

<span data-ttu-id="b59d8-122">下面的示例将升级聊天中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="b59d8-122">The following example upgrades an app installed in a chat.</span></span>
<!-- {
  "blockType": "request",
  "name": "upgrade_installedApps_in_chat"
}-->

```http
POST https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=/upgrade
```

### <a name="response"></a><span data-ttu-id="b59d8-123">响应</span><span class="sxs-lookup"><span data-stu-id="b59d8-123">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat update installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

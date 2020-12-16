---
title: teamsAppInstallation：升级
description: 更新聊天中安装的应用程序，并使其与租户应用目录中提供的当前版本保持同步。
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a3ab5c22a627513d811e3c61397bbd7511a1928
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658553"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="37f9e-103">teamsAppInstallation：升级</span><span class="sxs-lookup"><span data-stu-id="37f9e-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="37f9e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37f9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37f9e-105">升级[聊天](../resources/chat.md)中的[应用安装](../resources/teamsappinstallation.md)。</span><span class="sxs-lookup"><span data-stu-id="37f9e-105">Upgrade an [app installation](../resources/teamsappinstallation.md) within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="37f9e-106">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例相关联，然后，会议中安装的 **teamsApp** 将会迅速得到升级。</span><span class="sxs-lookup"><span data-stu-id="37f9e-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then effectively, the **teamsApp** installed in the meeting will get upgraded.</span></span>

## <a name="permissions"></a><span data-ttu-id="37f9e-107">权限</span><span class="sxs-lookup"><span data-stu-id="37f9e-107">Permissions</span></span>

<span data-ttu-id="37f9e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37f9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37f9e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="37f9e-110">Permission type</span></span>      | <span data-ttu-id="37f9e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="37f9e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37f9e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37f9e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="37f9e-113">TeamsAppInstallation.ReadWriteSelfForChat、TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="37f9e-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="37f9e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37f9e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37f9e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="37f9e-115">Not supported.</span></span>   |
|<span data-ttu-id="37f9e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="37f9e-116">Application</span></span> | <span data-ttu-id="37f9e-117">TeamsAppInstallation.ReadWriteSelfForChat.All、TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="37f9e-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37f9e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37f9e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /chats/{chat-id}/installedApps/{app-installation-id}/upgrade
```

## <a name="response"></a><span data-ttu-id="37f9e-119">响应</span><span class="sxs-lookup"><span data-stu-id="37f9e-119">Response</span></span>

<span data-ttu-id="37f9e-120">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="37f9e-120">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="37f9e-121">示例</span><span class="sxs-lookup"><span data-stu-id="37f9e-121">Example</span></span>

### <a name="request"></a><span data-ttu-id="37f9e-122">请求</span><span class="sxs-lookup"><span data-stu-id="37f9e-122">Request</span></span>

<span data-ttu-id="37f9e-123">下面的示例将升级聊天中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="37f9e-123">The following example upgrades an app installed in a chat.</span></span>
<!-- {
  "blockType": "request",
  "name": "upgrade_installedApps_in_chat"
}-->

```http
POST https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=/upgrade
```

### <a name="response"></a><span data-ttu-id="37f9e-124">响应</span><span class="sxs-lookup"><span data-stu-id="37f9e-124">Response</span></span>

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

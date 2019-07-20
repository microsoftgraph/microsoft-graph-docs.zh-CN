---
title: Microsoft Teams 中的受保护 API
description: Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ebf0bbda324f62c6413bbe3d70ade33a5052da0d
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778759"
---
# <a name="protected-apis-in-microsoft-teams"></a><span data-ttu-id="6fbda-103">Microsoft Teams 中的受保护 API</span><span class="sxs-lookup"><span data-stu-id="6fbda-103">Protected APIs in Microsoft Teams</span></span>

<span data-ttu-id="6fbda-104">Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。</span><span class="sxs-lookup"><span data-stu-id="6fbda-104">Microsoft Teams APIs in Microsoft Graph that access sensitive data are considered protected APIs.</span></span> <span data-ttu-id="6fbda-105">除了权限和许可之外，这些 API 还需要进行额外的验证，然后才能使用。</span><span class="sxs-lookup"><span data-stu-id="6fbda-105">These APIs require that you have additional validation, beyond permissions and consent, before you can use them.</span></span>

<span data-ttu-id="6fbda-106">以下是当前受保护的 API：</span><span class="sxs-lookup"><span data-stu-id="6fbda-106">The following APIs are currently protected:</span></span>
* <span data-ttu-id="6fbda-107">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出频道消息](/graph/api/channel-list-messages?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="6fbda-107">[List channel messages](/graph/api/channel-list-messages?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="6fbda-108">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取频道消息](/graph/api/channel-get-message?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="6fbda-108">[Get channel message](/graph/api/channel-get-message?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="6fbda-109">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出消息回复](/graph/api/channel-list-messagereplies?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="6fbda-109">[List replies to a message](/graph/api/channel-list-messagereplies?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="6fbda-110">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取消息回复](/graph/api/channel-get-messagereply?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="6fbda-110">[Get a reply to a message](/graph/api/channel-get-messagereply?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="6fbda-111">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出聊天中的消息](/graph/api/chatmessage-list?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="6fbda-111">[List messages in a chat](/graph/api/chatmessage-list?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="6fbda-112">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取聊天中的消息](/graph/api/chatmessage-get?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="6fbda-112">[Get message in chat](/graph/api/chatmessage-get?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>

<span data-ttu-id="6fbda-113">若要请求对这些受保护 API 的访问权限，请完成以下[请求表单](http://aka.ms/teamsgraph/requestaccess)。</span><span class="sxs-lookup"><span data-stu-id="6fbda-113">To request access to these protected APIs, complete the following [request form](http://aka.ms/teamsgraph/requestaccess).</span></span> <span data-ttu-id="6fbda-114">我们每周都会查看一次访问权限请求。</span><span class="sxs-lookup"><span data-stu-id="6fbda-114">We review access requests weekly.</span></span> <span data-ttu-id="6fbda-115">如果想要在表单之外提供其他信息，可与 [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com) 联系。</span><span class="sxs-lookup"><span data-stu-id="6fbda-115">If you would like to provide information in addition to the form, you can contact [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).</span></span>

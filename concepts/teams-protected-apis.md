---
title: Microsoft Teams 中的受保护 API
description: Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: b952e62e546093a7cc753c195fcd8c22db59d205
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734400"
---
# <a name="protected-apis-in-microsoft-teams"></a><span data-ttu-id="e6979-103">Microsoft Teams 中的受保护 API</span><span class="sxs-lookup"><span data-stu-id="e6979-103">Protected APIs in Microsoft Teams</span></span>

<span data-ttu-id="e6979-104">Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。</span><span class="sxs-lookup"><span data-stu-id="e6979-104">Microsoft Teams APIs in Microsoft Graph that access sensitive data are considered protected APIs.</span></span> <span data-ttu-id="e6979-105">除了权限和许可之外，这些 API 还需要进行额外的验证，然后才能使用。</span><span class="sxs-lookup"><span data-stu-id="e6979-105">These APIs require that you have additional validation, beyond permissions and consent, before you can use them.</span></span>

<span data-ttu-id="e6979-106">以下是当前受保护的 API：</span><span class="sxs-lookup"><span data-stu-id="e6979-106">The following APIs are currently protected:</span></span>
* <span data-ttu-id="e6979-107">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出频道消息](/graph/api/channel-list-messages?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="e6979-107">[List channel messages](/graph/api/channel-list-messages?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="e6979-108">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取频道增量中的聊天消息](/graph/api/chatmessage-delta?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="e6979-108">[Get chatMessages in a channel delta](/graph/api/chatmessage-delta?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="e6979-109">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取频道消息](/graph/api/channel-get-message?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="e6979-109">[Get channel message](/graph/api/channel-get-message?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="e6979-110">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出消息回复](/graph/api/channel-list-messagereplies?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="e6979-110">[List replies to a message](/graph/api/channel-list-messagereplies?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="e6979-111">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取消息回复](/graph/api/channel-get-messagereply?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="e6979-111">[Get a reply to a message](/graph/api/channel-get-messagereply?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="e6979-112">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出聊天中的消息](/graph/api/chatmessage-list?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="e6979-112">[List messages in a chat](/graph/api/chatmessage-list?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="e6979-113">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取聊天中的消息](/graph/api/chatmessage-get?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="e6979-113">[Get message in chat](/graph/api/chatmessage-get?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="e6979-114">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出所有托管内容](/graph/api/chatmessage-list-chatmessagehostedcontents?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="e6979-114">[List all hosted content](/graph/api/chatmessage-list-chatmessagehostedcontents?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="e6979-115">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取托管内容](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="e6979-115">[Get hosted content](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="e6979-116">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出聊天成员](/graph/api/conversationmember-list?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="e6979-116">[List chat members](/graph/api/conversationmember-list?view=graph-rest-beta)  using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="e6979-117">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取聊天成员](/graph/api/conversationmember-get?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="e6979-117">[Get chat member](/graph/api/conversationmember-get?view=graph-rest-beta)  using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>

>[!NOTE]
><span data-ttu-id="e6979-118">[发送消息](/graph/api/channel-post-messages?view=graph-rest-beta) API 不受保护。</span><span class="sxs-lookup"><span data-stu-id="e6979-118">[Send message](/graph/api/channel-post-messages?view=graph-rest-beta) is not a protected API.</span></span>

<span data-ttu-id="e6979-119">要请求访问这些受保护的 API，请填写下述[请求表单](http://aka.ms/teamsgraph/requestaccess)。</span><span class="sxs-lookup"><span data-stu-id="e6979-119">To request access to these protected APIs, complete the following [request form](http://aka.ms/teamsgraph/requestaccess).</span></span> <span data-ttu-id="e6979-120">我们每周三查看访问权限请求，每周五部署批准。</span><span class="sxs-lookup"><span data-stu-id="e6979-120">We review access requests every Wednesday and deploy approvals every Friday.</span></span>
<span data-ttu-id="e6979-121">如果除了表单，还想要提供其他信息，可与 [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com) 联系。</span><span class="sxs-lookup"><span data-stu-id="e6979-121">If you would like to provide information in addition to the form, you can contact [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).</span></span>

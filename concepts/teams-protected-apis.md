---
title: Microsoft Teams 中的受保护 API
description: Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: dd4b2a85fd0ab3b9fbceb993cfd72ef5bf19f48b
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941429"
---
# <a name="protected-apis-in-microsoft-teams"></a><span data-ttu-id="7cfa8-103">Microsoft Teams 中的受保护 API</span><span class="sxs-lookup"><span data-stu-id="7cfa8-103">Protected APIs in Microsoft Teams</span></span>

<span data-ttu-id="7cfa8-104">Microsoft Graph 中用于访问敏感数据的 Microsoft Teams API 被视为受保护 API。</span><span class="sxs-lookup"><span data-stu-id="7cfa8-104">Microsoft Teams APIs in Microsoft Graph that access sensitive data are considered protected APIs.</span></span> <span data-ttu-id="7cfa8-105">除了权限和许可之外，这些 API 还需要进行额外的验证，然后才能使用。</span><span class="sxs-lookup"><span data-stu-id="7cfa8-105">These APIs require that you have additional validation, beyond permissions and consent, before you can use them.</span></span>


<span data-ttu-id="7cfa8-106">以下是当前受保护的 API：</span><span class="sxs-lookup"><span data-stu-id="7cfa8-106">The following APIs are currently protected:</span></span>
* <span data-ttu-id="7cfa8-107">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出频道消息](/graph/api/channel-list-messages)</span><span class="sxs-lookup"><span data-stu-id="7cfa8-107">[List channel messages](/graph/api/channel-list-messages) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="7cfa8-108">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取频道增量中的聊天消息](/graph/api/chatmessage-delta)</span><span class="sxs-lookup"><span data-stu-id="7cfa8-108">[Get chatMessages in a channel delta](/graph/api/chatmessage-delta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="7cfa8-109">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取频道消息](/graph/api/chatmessage-get)</span><span class="sxs-lookup"><span data-stu-id="7cfa8-109">[Get channel message](/graph/api/chatmessage-get) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="7cfa8-110">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)[创建新频道消息订阅](/graph/api/subscription-post-subscriptions)</span><span class="sxs-lookup"><span data-stu-id="7cfa8-110">[Create subscription for new channel messages](/graph/api/subscription-post-subscriptions) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="7cfa8-111">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出消息回复](/graph/api/chatmessage-list-replies)</span><span class="sxs-lookup"><span data-stu-id="7cfa8-111">[List replies to a message](/graph/api/chatmessage-list-replies) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="7cfa8-112">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取消息回复](/graph/api/chatmessage-get)</span><span class="sxs-lookup"><span data-stu-id="7cfa8-112">[Get a reply to a message](/graph/api/chatmessage-get) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="7cfa8-113">（使用不存在的[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)列出聊天，带或不带受保护的 API 权限）</span><span class="sxs-lookup"><span data-stu-id="7cfa8-113">(List chats using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions) doesn't exist, with or without protected API access)</span></span>
* <span data-ttu-id="7cfa8-114">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出聊天中的消息](/graph/api/chat-list-messages)</span><span class="sxs-lookup"><span data-stu-id="7cfa8-114">[List messages in a chat](/graph/api/chat-list-messages) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="7cfa8-115">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取聊天中的消息](/graph/api/chatmessage-get)</span><span class="sxs-lookup"><span data-stu-id="7cfa8-115">[Get message in chat](/graph/api/chatmessage-get) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="7cfa8-116">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)[创建新聊天消息订阅](/graph/api/subscription-post-subscriptions)</span><span class="sxs-lookup"><span data-stu-id="7cfa8-116">[Create subscription for new chat messages](/graph/api/subscription-post-subscriptions) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="7cfa8-117">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[列出所有托管内容](/graph/api/chatmessage-list-hostedcontents)</span><span class="sxs-lookup"><span data-stu-id="7cfa8-117">[List all hosted content](/graph/api/chatmessage-list-hostedcontents) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="7cfa8-118">使用[应用程序权限](auth/auth-concepts.md#microsoft-graph-permissions)的[获取托管内容](/graph/api/chatmessagehostedcontent-get)</span><span class="sxs-lookup"><span data-stu-id="7cfa8-118">[Get hosted content](/graph/api/chatmessagehostedcontent-get) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>

>[!NOTE]
><span data-ttu-id="7cfa8-119">[发送消息](/graph/api/channel-post-messages) API 不受保护。</span><span class="sxs-lookup"><span data-stu-id="7cfa8-119">[Send message](/graph/api/channel-post-messages) is not a protected API.</span></span>

<span data-ttu-id="7cfa8-120">要请求访问这些受保护的 API，请填写下述[请求表单](https://aka.ms/teamsgraph/requestaccess)。</span><span class="sxs-lookup"><span data-stu-id="7cfa8-120">To request access to these protected APIs, complete the following [request form](https://aka.ms/teamsgraph/requestaccess).</span></span> <span data-ttu-id="7cfa8-121">我们在每周三审查访问请求，并在每周五部署批准，但美国的主要节假日周除外。在这些周中的提交将在下一个非节假日周进行处理。</span><span class="sxs-lookup"><span data-stu-id="7cfa8-121">We review access requests every Wednesday and deploy approvals every Friday, except during major holiday weeks in the U.S. Submissions during those weeks will be processed the following non-holiday week.</span></span>

<span data-ttu-id="7cfa8-122">如果除了表单，还想要提供其他信息，可与 [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com) 联系。</span><span class="sxs-lookup"><span data-stu-id="7cfa8-122">If you would like to provide information in addition to the form, you can contact [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).</span></span>

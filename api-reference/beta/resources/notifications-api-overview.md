---
title: 使用 Microsoft Graph 的通知 REST API
description: 你可以使用 Microsoft Graph 中的通知 API 向用户发送推送通知。 。
localization_priority: Priority
ms.prod: notifications
doc_type: conceptualPageType
author: merzink
ms.openlocfilehash: 9579f4856273a6d9ccae6fb45f2956be13f8435d
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405091"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a><span data-ttu-id="ba76a-104">使用 Microsoft Graph 的通知 REST API</span><span class="sxs-lookup"><span data-stu-id="ba76a-104">Use the notifications REST API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba76a-105">你可以使用 Microsoft Graph 中的通知 API 向用户发送推送通知。</span><span class="sxs-lookup"><span data-stu-id="ba76a-105">You can use the notifications API in Microsoft Graph to send push notifications to a user.</span></span> <span data-ttu-id="ba76a-106">只需向目标用户发布通知，平台即可向注册到该用户的所有设备终结点发送通知。</span><span class="sxs-lookup"><span data-stu-id="ba76a-106">Simply post a notification to your target user, and the platform will deliver the notification to all device endpoints registered to that user.</span></span> <span data-ttu-id="ba76a-107">高级流如下所示：</span><span class="sxs-lookup"><span data-stu-id="ba76a-107">The high-level flow is as follows:</span></span>

1. <span data-ttu-id="ba76a-108">用户登录到你的应用程序，从而创建包含 Microsoft Graph 通知服务的订阅。</span><span class="sxs-lookup"><span data-stu-id="ba76a-108">User signs in to your application, which creates a subscription with the Microsoft Graph notification service.</span></span> <span data-ttu-id="ba76a-109">将向调用应用程序返回特定用户通知订阅 ID 或 UNSID。</span><span class="sxs-lookup"><span data-stu-id="ba76a-109">A specific user notification subscription ID or UNSID will be returned to the calling application.</span></span>
2. <span data-ttu-id="ba76a-110">应用程序将此 UNSID 发送到应用程序服务。</span><span class="sxs-lookup"><span data-stu-id="ba76a-110">The application sends this UNSID to your application service.</span></span>
3. <span data-ttu-id="ba76a-111">准备好发送通知时，应用程序服务[通过 Microsoft 标识平台进行身份验证](/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow)，并通过 Microsoft Graph 通知服务发布通知，提供验证码、目标用户的 UNSID 以及通知负载。</span><span class="sxs-lookup"><span data-stu-id="ba76a-111">When ready to send a notification, your application service [authenticates with the Microsoft identity platform](/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow) and posts a notification via the Microsoft Graph notification service, providing the auth token, target user's UNSID, and notification payload.</span></span>
4. <span data-ttu-id="ba76a-112">Microsoft Graph 通知服务将通知扇出至具有活动订阅的用户的所有终结点。</span><span class="sxs-lookup"><span data-stu-id="ba76a-112">The Microsoft Graph notification service fans-out notifications to all endpoints of the user with an active subscription.</span></span>  

<span data-ttu-id="ba76a-113">此类以用户为中心的通知通过 [](../resources/projectrome-notification.md) 资源标识，存储在 Microsoft Graph 通知服务中。</span><span class="sxs-lookup"><span data-stu-id="ba76a-113">This type of user-centric notification is represented by the [notification](../resources/projectrome-notification.md) resource and is stored within the Microsoft Graph notification service.</span></span> <span data-ttu-id="ba76a-114">随后可由客户端应用程序通过[客户端 SDK API](https://aka.ms/GNSDK) 访问和管理。</span><span class="sxs-lookup"><span data-stu-id="ba76a-114">It can then be accessed and managed by the client application via the [client-side SDK APIs](https://aka.ms/GNSDK).</span></span> <span data-ttu-id="ba76a-115">若不熟悉 Microsoft Graph 通知服务，请查看[通知概述](/graph/notifications-concept-overview)部分了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="ba76a-115">If you're new to the Microsoft Graph notification service, check out the [notification overview](/graph/notifications-concept-overview) section to learn more.</span></span>    

## <a name="whats-new"></a><span data-ttu-id="ba76a-116">最近更新</span><span class="sxs-lookup"><span data-stu-id="ba76a-116">What's new</span></span>
<span data-ttu-id="ba76a-117">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="ba76a-117">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ba76a-118">后续步骤</span><span class="sxs-lookup"><span data-stu-id="ba76a-118">Next steps</span></span>
- <span data-ttu-id="ba76a-119">请参阅[通知资源](../resources/projectrome-notification.md)并创建通知，以与用户交互。</span><span class="sxs-lookup"><span data-stu-id="ba76a-119">See the [notification resource](../resources/projectrome-notification.md) and create notifications to engage with your users.</span></span> 
- <span data-ttu-id="ba76a-120">在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。</span><span class="sxs-lookup"><span data-stu-id="ba76a-120">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="ba76a-121">按照[集成概述](/graph/notifications-integration-e2e-overview)主题中的步骤开始客户端集成。</span><span class="sxs-lookup"><span data-stu-id="ba76a-121">Get started with client integration by following the steps in the [integration overview](/graph/notifications-integration-e2e-overview) topic.</span></span>
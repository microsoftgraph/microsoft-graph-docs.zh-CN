---
title: 通过应用程序服务创建和发送通知
description: '将应用程序服务设置为通过 Microsoft Graph 向不同客户端发送以用户为中心的通知。 '
localization_priority: Priority
ms.prod: notifications
author: merzink
ms.openlocfilehash: d430622d05337cdb00f29de316d5d5cd948e1e05
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37934349"
---
# <a name="create-and-send-a-notification-from-your-app-service"></a><span data-ttu-id="db265-103">通过应用程序服务创建和发送通知</span><span class="sxs-lookup"><span data-stu-id="db265-103">Create and send a notification from your app service</span></span>

<span data-ttu-id="db265-104">可以使用 Microsoft Graph API 为用户创建和发送通知。</span><span class="sxs-lookup"><span data-stu-id="db265-104">You can create and send a notification to a user by using Microsoft Graph APIs.</span></span> <span data-ttu-id="db265-105">通知存储在 Microsoft Graph 通知服务中，并发送到目标用户登录的所有设备上的所有应用客户端。</span><span class="sxs-lookup"><span data-stu-id="db265-105">The notification is stored in the activity feed store and is sent to all app clients on all devices that the target user is signed in on.</span></span> 

<span data-ttu-id="db265-106">若要向你的用户发送通知，你的应用程序服务将：</span><span class="sxs-lookup"><span data-stu-id="db265-106">In order to send a notification to your user, your application service will:</span></span>
1. <span data-ttu-id="db265-107">向 Microsoft 标识平台[进行身份验证](/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow)。</span><span class="sxs-lookup"><span data-stu-id="db265-107">[Authenticate](/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow) with the Microsoft identity platform.</span></span>
2. <span data-ttu-id="db265-108">使用身份验证令牌将通知发布到 Microsoft Graph API，并以[用户通知订阅 ID](/graph/api/notifications-post)（创建订阅时从应用客户端获取）定位用户。</span><span class="sxs-lookup"><span data-stu-id="db265-108">Post a notification to the Microsoft Graph API using the auth token, and target the user with a [user notification subscription ID](/graph/api/notifications-post) that is obtained from your app client when creating a subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="db265-109">为获得简化的身份验证故事，建议使用客户端上新的和改进的轻型[通知 SDK](https://aka.ms/GNSDK) 以及用户通知订阅 ID 来接收通知和管理通知状态。</span><span class="sxs-lookup"><span data-stu-id="db265-109">For a simplified authentication story, we recommend using the new and improved, lightweight [notification SDK](https://aka.ms/GNSDK) on the client-side with a user notification subscription ID to receive notifications and manage notification state.</span></span> <span data-ttu-id="db265-110">或者，你可以通过委派权限代表用户发布通知，你的应用服务将需要维护访问令牌和刷新令牌，但不建议这样做。</span><span class="sxs-lookup"><span data-stu-id="db265-110">Alternatively, you can  post notifications on behalf of the user via delegated permissions and your app service will need to maintain access tokens and refresh tokens, but this is not recommended.</span></span> <span data-ttu-id="db265-111">若要详细了解 OAuth 2.0 OBO 流，请参阅[代表流中使用委派用户标识的服务到服务调用](https://docs.microsoft.com/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow)。</span><span class="sxs-lookup"><span data-stu-id="db265-111">To learn more about OAuth 2.0 OBO flow, see [Service-to-service calls that use delegated user identity in the On-Behalf-Of flow](https://docs.microsoft.com/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow).</span></span> 


## <a name="guaranteed-delivery-on-ios"></a><span data-ttu-id="db265-112">iOS 上的保证传递</span><span class="sxs-lookup"><span data-stu-id="db265-112">Guaranteed delivery on iOS</span></span>

<span data-ttu-id="db265-113">在如 iOS 的平台上，在特定电源条件下，原始数据通知可能由于批处理而延迟传递，或者根本无法到达目标终结点。</span><span class="sxs-lookup"><span data-stu-id="db265-113">On platforms like iOS, under certain power conditions, raw data notifications might be delayed in delivery due to batching, or not reach the target endpoint at all.</span></span> <span data-ttu-id="db265-114">为了向 iOS 上的用户传递高优先级通知，Microsoft Graph 通知平台允许你指定原始到可视 toast 通知“回退”选项，该选项会自动向目标 iOS 设备发送可视 toast 通知，从而确保你的用户近实时获得通知。</span><span class="sxs-lookup"><span data-stu-id="db265-114">For high-priority notifications being delivered to users on iOS, the Microsoft Graph notifications platform allows you to specify a raw-to-visual toast notification "fallback" option that automatically sends a visual toast notification to the target iOS device, thereby ensuring your user gets notified near real-time.</span></span> <span data-ttu-id="db265-115">若要了解如何利用回退选项，请参阅[通知资源](/graph/api/resources/projectrome-notification.md)。</span><span class="sxs-lookup"><span data-stu-id="db265-115">To learn how to leverage fallback options, please see the [notification resource](/graph/api/resources/projectrome-notification.md).</span></span>  

## <a name="getting-started"></a><span data-ttu-id="db265-116">入门</span><span class="sxs-lookup"><span data-stu-id="db265-116">Getting started</span></span>
<span data-ttu-id="db265-117">若要了解你的应用服务如何开始向你的用户发送通知，请参阅[通知](/graph/api/resources/projectrome-notification)和我们的[应用服务示例](https://aka.ms/gnsample-appservice)。</span><span class="sxs-lookup"><span data-stu-id="db265-117">To learn how your app service can start sending notifications to your users, see [notification](/graph/api/resources/projectrome-notification) and our [App Service sample](https://aka.ms/gnsample-appservice).</span></span>

---
title: 通过应用程序服务创建和发送通知
description: '将应用程序服务设置为通过 Microsoft Graph 向不同客户端发送以用户为中心的通知。 '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: cf40087aff3956a88f79197482db8126bbe8d96c
ms.sourcegitcommit: 895a03cb2706a9b3a2236b30d6a7e9f5cbc6a89e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34683508"
---
# <a name="create-and-send-a-notification-from-your-app-service"></a><span data-ttu-id="58b3f-103">通过应用程序服务创建和发送通知</span><span class="sxs-lookup"><span data-stu-id="58b3f-103">Create and send a notification from your app service</span></span>

<span data-ttu-id="58b3f-104">可以使用 Microsoft Graph API 为用户创建和发送通知。</span><span class="sxs-lookup"><span data-stu-id="58b3f-104">You can create and send a notification to a user by using Microsoft Graph APIs.</span></span> <span data-ttu-id="58b3f-105">通知存储在活动源存储中，并发送到目标用户登录的所有设备上的所有应用客户端。</span><span class="sxs-lookup"><span data-stu-id="58b3f-105">The notification is stored in the activity feed store and is sent to all app clients on all devices that the target user is signed in on.</span></span> 

## <a name="authentication"></a><span data-ttu-id="58b3f-106">身份验证</span><span class="sxs-lookup"><span data-stu-id="58b3f-106">Authentication</span></span>

<span data-ttu-id="58b3f-107">Microsoft Graph 通知要求你的应用程序服务使用代表 (OBO) 流向用户发布通知。</span><span class="sxs-lookup"><span data-stu-id="58b3f-107">Microsoft Graph notifications requires that your application service uses the On-Behalf-Of (OBO) flow to post a notification to a user.</span></span> <span data-ttu-id="58b3f-108">以下是身份验证流：</span><span class="sxs-lookup"><span data-stu-id="58b3f-108">The following is a simple and typical authentication flow:</span></span>

1.  <span data-ttu-id="58b3f-109">用户使用其 Microsoft 或工作或学校帐户登录至你的应用程序。</span><span class="sxs-lookup"><span data-stu-id="58b3f-109">The user signs in to your application with their Microsoft or their work or school account.</span></span> <span data-ttu-id="58b3f-110">登录时，标识服务将为你提供一个访问令牌。</span><span class="sxs-lookup"><span data-stu-id="58b3f-110">When they sign in, the identity service gives you an access token.</span></span>

2.  <span data-ttu-id="58b3f-111">你将此访问令牌发送至应用程序服务。</span><span class="sxs-lookup"><span data-stu-id="58b3f-111">You send the access token to your app service.</span></span>

3.  <span data-ttu-id="58b3f-112">应用程序服务对标识服务进行身份验证，并且需要 OBO 令牌才能发送 Microsoft Graph 通知。</span><span class="sxs-lookup"><span data-stu-id="58b3f-112">You app service authenticates against the identity service and requests an OBO token for Microsoft Graph notifications.</span></span>

4.  <span data-ttu-id="58b3f-113">标识服务返回基于 OBO 的令牌和刷新令牌。</span><span class="sxs-lookup"><span data-stu-id="58b3f-113">The identity service returns an OBO-based token and a refresh token.</span></span> <span data-ttu-id="58b3f-114">应用程序服务可以使用此访问令牌向用户发布通知。</span><span class="sxs-lookup"><span data-stu-id="58b3f-114">Your app service can use this access token to post notifications to this user.</span></span>

<span data-ttu-id="58b3f-115">若要详细了解 OAuth 2.0 OBO 流，请参阅[代表流中使用委派用户标识的服务到服务调用](https://docs.microsoft.com/en-us/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow)。</span><span class="sxs-lookup"><span data-stu-id="58b3f-115">To learn more about OAuth 2.0 OBO flow, see [Service-to-service calls that use delegated user identity in the On-Behalf-Of flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow).</span></span> <span data-ttu-id="58b3f-116">有关此流与 Microsoft Graph 通知如何搭配使用的详细信息，请参阅[应用程序服务示例](https://aka.ms/gnsample-appservice)。</span><span class="sxs-lookup"><span data-stu-id="58b3f-116">For details about how this flow works with Microsoft Graph notifications, see the [App Service sample](https://aka.ms/gnsample-appservice).</span></span>

> [!NOTE]
> <span data-ttu-id="58b3f-117">Microsoft Graph 通知目前使用带有未来计划的 OBO 身份验证流，以此进一步简化此身份验证，并消除维护访问令牌和刷新令牌的需要。</span><span class="sxs-lookup"><span data-stu-id="58b3f-117">Microsoft Graph notifications currently uses OBO authentication flow with future plans to simplify this authentication further and eliminate the need to maintain access tokens and refresh tokens.</span></span>

<span data-ttu-id="58b3f-118">有关 API 权限以及请求和响应标题的更多详细信息，请参阅 API 参考部分的[创建和发送通知](/graph/api/notifications-post)。</span><span class="sxs-lookup"><span data-stu-id="58b3f-118">For more details on the API permissions and on the request and response headers, please see [Create and send a notification](/graph/api/notifications-post) in the API reference section.</span></span> 

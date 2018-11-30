---
title: 在 Microsoft Graph 中使用 REST API 的通知
description: 在 Microsoft Graph 中的通知 API 可用于向用户发送推送通知。 只需目标的用户帐户以发送通知，以及在平台将传递到所有设备终结点的通知。 通知 API 请求执行代表通过委派的权限和[通知的权限]( /graph/permissions_reference)，用户可用于或者是 Microsoft 帐户或工作或学校帐户。
ms.openlocfilehash: 07b59fb7d7eae2e626b58325e82999bbd36c5489
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044857"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a><span data-ttu-id="840f9-105">在 Microsoft Graph 中使用 REST API 的通知</span><span class="sxs-lookup"><span data-stu-id="840f9-105">Use the notifications REST API in Microsoft Graph</span></span>

> <span data-ttu-id="840f9-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="840f9-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="840f9-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="840f9-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="840f9-108">在 Microsoft Graph 中的通知 API 可用于向用户发送推送通知。</span><span class="sxs-lookup"><span data-stu-id="840f9-108">You can use the notifications API in Microsoft Graph to send push notifications to a user.</span></span> <span data-ttu-id="840f9-109">只需目标的用户帐户以发送通知，以及在平台将传递到所有设备终结点的通知。</span><span class="sxs-lookup"><span data-stu-id="840f9-109">Simply target a user account to send a notification to, and the platform will deliver the notification to all device endpoints.</span></span> <span data-ttu-id="840f9-110">通知 API 请求执行代表通过[委派权限](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions)和[通知的权限]( /graph/permissions_reference)，用户可用于或者是 Microsoft 帐户或工作或学校帐户。</span><span class="sxs-lookup"><span data-stu-id="840f9-110">Notifications API requests are performed on behalf of a user via [delegated permissions](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) and the [notification permission]( /graph/permissions_reference), which can be used with either Microsoft accounts or work or school accounts.</span></span>
<span data-ttu-id="840f9-111">以用户为中心的通知的此类型由[通知](../resources/projectrome-notification.md)资源，存储在 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="840f9-111">This type of user-centric notification is represented by the [notification](../resources/projectrome-notification.md) resource and is stored in Microsoft Graph.</span></span> <span data-ttu-id="840f9-112">它可以然后访问和管理发布应用程序通过[项目 Rome SDK Api](https://github.com/Microsoft/project-rome)。</span><span class="sxs-lookup"><span data-stu-id="840f9-112">It can then be accessed and managed by the publishing app via the [Project Rome SDK APIs](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="next-steps"></a><span data-ttu-id="840f9-113">后续步骤</span><span class="sxs-lookup"><span data-stu-id="840f9-113">Next steps</span></span>
- <span data-ttu-id="840f9-114">请参阅[通知资源](../resources/projectrome-notification.md)和创建通知来与您的用户。</span><span class="sxs-lookup"><span data-stu-id="840f9-114">See the [notification resource](../resources/projectrome-notification.md) and create notifications to engage with your users.</span></span> 
- <span data-ttu-id="840f9-115">尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中使用 API。</span><span class="sxs-lookup"><span data-stu-id="840f9-115">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

---
title: 使用 Microsoft Graph 的通知 REST API
description: 你可以使用 Microsoft Graph 中的通知 API 向用户发送推送通知。 只需定位要向其发送通知的用户帐户，平台即可向所有设备终结点发送通知。 将通过委派权限和[通知权限]( /graph/permissions_reference)代表用户执行通知 API 请求，这两种权限可与 Microsoft 帐户或工作或学校帐户结合使用。
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 243f412162ed1427c766272d02d58c57ba47cf42
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342098"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a><span data-ttu-id="cf01b-105">使用 Microsoft Graph 的通知 REST API</span><span class="sxs-lookup"><span data-stu-id="cf01b-105">Use the notifications REST API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf01b-106">你可以使用 Microsoft Graph 中的通知 API 向用户发送推送通知。</span><span class="sxs-lookup"><span data-stu-id="cf01b-106">You can use the notifications API in Microsoft Graph to send push notifications to a user.</span></span> <span data-ttu-id="cf01b-107">只需定位要向其发送通知的用户帐户，平台即可向所有设备终结点发送通知。</span><span class="sxs-lookup"><span data-stu-id="cf01b-107">Simply target a user account to send a notification to, and the platform will deliver the notification to all device endpoints.</span></span> <span data-ttu-id="cf01b-108">将通过[委派权限](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions)和[通知权限]( /graph/permissions_reference)代表用户执行通知 API 请求，这两种权限可与 Microsoft 帐户或工作或学校帐户结合使用。</span><span class="sxs-lookup"><span data-stu-id="cf01b-108">Notifications API requests are performed on behalf of a user via [delegated permissions](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) and the [notification permission]( /graph/permissions_reference), which can be used with either Microsoft accounts or work or school accounts.</span></span>
<span data-ttu-id="cf01b-109">此类以用户为中心的通知通过[通知](../resources/projectrome-notification.md)资源标识，存储在 Microsoft Graph 中。</span><span class="sxs-lookup"><span data-stu-id="cf01b-109">This type of user-centric notification is represented by the [notification](../resources/projectrome-notification.md) resource and is stored in Microsoft Graph.</span></span> <span data-ttu-id="cf01b-110">随后可由发布应用程序通过 [Project Rome SDK API](https://github.com/Microsoft/project-rome) 访问和管理。</span><span class="sxs-lookup"><span data-stu-id="cf01b-110">It can then be accessed and managed by the publishing app via the [Project Rome SDK APIs](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="next-steps"></a><span data-ttu-id="cf01b-111">后续步骤</span><span class="sxs-lookup"><span data-stu-id="cf01b-111">Next steps</span></span>
- <span data-ttu-id="cf01b-112">请参阅[通知资源](../resources/projectrome-notification.md)并创建通知，以与用户交互。</span><span class="sxs-lookup"><span data-stu-id="cf01b-112">See the [notification resource](../resources/projectrome-notification.md) and create notifications to engage with your users.</span></span> 
- <span data-ttu-id="cf01b-113">尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。</span><span class="sxs-lookup"><span data-stu-id="cf01b-113">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

---
title: '使用 Microsoft Graph 中的通知 API 实现以人为中心的通知体验 '
description: '通知是重新吸引用户的最为有效的方式。 它们可以吸引用户的注意力并将用户重新吸引到你的应用中。 在多设备环境中，用户可以在任意地点，从应用所在的不同平台和设备访问应用和服务。 '
ms.openlocfilehash: 7ff36d7e0d406cb7918e2999812e3c756ae3b5bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091794"
---
# <a name="using-the-notifications-api-in-microsoft-graph-to-enable-human-centric-notification-experiences"></a>使用 Microsoft Graph 中的通知 API 实现以人为中心的通知体验 

通知是重新吸引用户的最为有效的方式。 它们可以吸引用户的注意力并将用户重新吸引到你的应用中。 在多设备环境中，用户可以在任意地点，从应用所在的不同平台和设备访问应用和服务。 

通知方案应本着“以人为中心”的方式进行设计，其主要目标是通知用户，而无论用户身处何地。 由主要平台提供的现有通知解决方案非常适合定位设备。 Microsoft Graph 通知通过允许你定位用户来改进此功能。 Microsoft Graph 通知将负责执行这一繁重的任务，其中包括在用户和终结点之间映射、跨用户的不同终结点同步通知状态等。 

## <a name="why-integrate-with-microsoft-graph-notifications"></a>为什么与 Microsoft Graph 通知集成？
### <a name="deliver-notifications-to-a-user-across-different-endpoints"></a>跨不同终结点向用户传递通知
作为 Microsoft Graph 的一部分，通知 API 允许你定位 Microsoft 帐户或工作或学校 (Azure AD) 帐户以传递通知。 平台将此通知分发给所有用户的终结点，其中包括 Windows UWP、Android 和 iOS。 

### <a name="manage-notifications-across-endpoints"></a>管理跨终结点的通知
Microsoft Graph 通知 API 允许你更新通知的状态并在所有终结点上同步该状态。 例如，当用户对一个设备上的通知执行操作时，你可以更新此通知的状态（例如将其设置为已读或已消除），并向所有其他终结点分发同一状态更改。 Microsoft Graph 通知 API 以集中式方式跟踪用户通知的状态，以便能够轻松地确保只需对通知进行一次处理即可在任意位置消除这些通知。

### <a name="retrieve-notification-history"></a>检索通知历史记录
可以使用通知 API 基于所定义的过期时间（最多 30 天）来检索通知历史记录。 标记为已读或已消除的通知仍然可从历史记录中检索，支持通知历史记录和其他方案的应用内视图。 

## <a name="integrating-with-the-notifications-api-in-microsoft-graph"></a>与 Microsoft Graph 中的通知 API 集成

只需执行几个简单的步骤即可将应用与 Microsoft Graph 通知集成：通过 Windows 开发人员中心载入应用、使用[创建通知](/graph/api/projectrome-notification-post?view=graph-rest-beta)方法发布通知，然后使用 Project Rome SDK 接收和管理应用客户端上的通知。  

若要详细了解如何通过 Microsoft Graph 发布用户通知，请参阅[通知 API 参考](/graph/api/resources/notifications-api-overview?view=graph-rest-beta)。
 
若要了解通过与 Project Rome SDK 集成接收和管理通知的详细信息，请参阅 [Project Rome SDK 文档](https://docs.microsoft.com/zh-CN/windows/project-rome/) 

## <a name="see-also"></a>另请参阅

- [Microsoft Graph 中的跨设备体验](cross-device-concept-overview.md)
- [Project Rome 开发人员中心](https://aka.ms/projectrome)

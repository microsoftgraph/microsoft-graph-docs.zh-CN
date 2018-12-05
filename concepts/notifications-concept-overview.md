---
title: '使用通知 API 在 Microsoft Graph 中的启用 human 中心通知体验 '
description: '通知是最有效的方式来重新与您的用户。 他们可以捕获用户的注意，并将恢复到您的应用程序的用户。 在多设备世界中，用户可以访问您的应用程序和服务从任何位置，跨不同平台和您的应用程序其中拥有状态的设备。 '
ms.openlocfilehash: 7ff36d7e0d406cb7918e2999812e3c756ae3b5bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091794"
---
# <a name="using-the-notifications-api-in-microsoft-graph-to-enable-human-centric-notification-experiences"></a>使用通知 API 在 Microsoft Graph 中的启用 human 中心通知体验 

通知是最有效的方式来重新与您的用户。 他们可以捕获用户的注意，并将恢复到您的应用程序的用户。 在多设备世界中，用户可以访问您的应用程序和服务从任何位置，跨不同平台和您的应用程序其中拥有状态的设备。 

通知方案的设计应方式"human 中心"，在其中的主要目标是通知用户，无论它他/她位于何处。 提供的主要平台的现有通知解决方案是在面向设备极好。 Microsoft Graph 通知对此改进可允许您向目标用户。 Microsoft Graph 通知将负责繁重，包括用户和用户的不同的终结点和更多同步通知状态的终结点之间的映射。 

## <a name="why-integrate-with-microsoft-graph-notifications"></a>为什么将 Microsoft Graph 通知集成？
### <a name="deliver-notifications-to-a-user-across-different-endpoints"></a>跨不同的终结点发送给用户的通知
作为 Microsoft Graph 的一部分，通知 API 允许您针对 Microsoft 帐户或单位电话或学校 (Azure AD) 帐户发送通知。 平台分发到所有用户的终结点，包括 Windows UWP、 Android 和 iOS 此通知。 

### <a name="manage-notifications-across-endpoints"></a>管理通知个终结点
Microsoft Graph 通知 API 可以更新通知的状态并跨所有终结点进行同步的状态。 例如，当用户对设备上的通知，您可以更新的状态 （例如，将其标记为已读或已消除），此通知和相同的状态更改将被分发给所有其他终结点。 Microsoft Graph 通知 API 跟踪状态的用户的通知方式集中，使您方便地确保您通知，一次处理并消除无处不在。

### <a name="retrieve-notification-history"></a>检索通知历史记录
通知 API 可用于检索基于过期时间定义 （最多 30 天） 的通知历史记录。 标记为通知读取或消除仍可检索从历史记录，启用通知历史记录和其他方案的应用程序内视图。 

## <a name="integrating-with-the-notifications-api-in-microsoft-graph"></a>与通知 API 在 Microsoft Graph 中集成

您可以将 Microsoft Graph 通知一些简单的步骤与-加载与您的应用程序集成您的应用程序通过 Windows 开发人员中心、[创建通知](/graph/api/projectrome-notification-post?view=graph-rest-beta)方法用于发布通知和使用 Project Rome SDK 接收和管理通知在您的应用程序的客户端。  

若要了解有关如何发布通过 Microsoft Graph 用户通知的详细信息，请参阅[通知 API 参考](/graph/api/resources/notifications-api-overview?view=graph-rest-beta)。
 
若要了解有关接收并通过将与 Project Rome SDK 集成管理通知的详细信息，请参阅[Project Rome SDK 文档](https://docs.microsoft.com/en-us/windows/project-rome/) 

## <a name="see-also"></a>另请参阅

- [Microsoft Graph 中的跨设备体验](cross-device-concept-overview.md)
- [项目 Rome 开发中心](https://aka.ms/projectrome)

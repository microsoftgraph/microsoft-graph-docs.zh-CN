---
title: '与 Microsoft Graph 通知集成 '
description: '通知是与应用程序用户再次交互的最有效的方式之一。 可以通过几个简单的步骤将应用程序与 Microsoft Graph 通知集成。  '
localization_priority: Priority
ms.prod: notifications
author: merzink
ms.openlocfilehash: 3cbeedfae4e47ac388b60d150505e247534ee68a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939571"
---
# <a name="integrate-with-microsoft-graph-notifications"></a><span data-ttu-id="ec296-104">与 Microsoft Graph 通知集成</span><span class="sxs-lookup"><span data-stu-id="ec296-104">Integrate with Microsoft Graph notifications</span></span>

<span data-ttu-id="ec296-105">可以通过几个简单的步骤（如下图所示）将应用程序与 Microsoft Graph 通知集成。</span><span class="sxs-lookup"><span data-stu-id="ec296-105">You can integrate your apps with Microsoft Graph notifications with a few simple steps, as shown in the following diagram.</span></span>

![显示载入通知步骤的图片：注册、跨设备载入、服务器集成和客户端集成](images/notifications-integration-e2e-overview.png)

1.  <span data-ttu-id="ec296-107">在 Microsoft Azure 门户中[注册](notifications-integration-app-registration.md)应用程序。</span><span class="sxs-lookup"><span data-stu-id="ec296-107">[Register](notifications-integration-app-registration.md) your application in the Microsoft Azure portal.</span></span>

2. <span data-ttu-id="ec296-108">[载入](notifications-integration-cross-device-experiences-onboarding.md)到合作伙伴中心/Windows 开发人员中心，以获取 Windows、iOS 和 Android 的跨平台应用程序标识和推送通知凭据。</span><span class="sxs-lookup"><span data-stu-id="ec296-108">[Onboard](notifications-integration-cross-device-experiences-onboarding.md) to Partner Center/Windows Dev Center for cross-platform application identity and push notification credentials.</span></span>

3.  <span data-ttu-id="ec296-109">[将应用程序服务器](notifications-integrating-app-server.md)设置为通过 Microsoft Graph 发送通知。</span><span class="sxs-lookup"><span data-stu-id="ec296-109">[Set up your app server](notifications-integrating-app-server.md) to send notifications via Microsoft Graph.</span></span>

4.  <span data-ttu-id="ec296-110">[将](notifications-integrating-with-windows.md)新的[通知客户端 SDK](https://aka.ms/GNSDK) 集成到 Windows、iOS、Android 或 Web 客户端，以接收和管理通知。</span><span class="sxs-lookup"><span data-stu-id="ec296-110">[Integrate](notifications-integrating-with-windows.md) the [Microsoft Graph notifications client SDK](https://aka.ms/GNSDK) into your Windows, Android, or iOS app clients to receive and manage notifications.</span></span>

> [!NOTE]
> <span data-ttu-id="ec296-111">我们建议使用新增和改进的轻型[通知 SDK](https://aka.ms/GNSDK)，而不是跨设备 [Project Rome SDK](https://github.com/microsoft/project-rome)。</span><span class="sxs-lookup"><span data-stu-id="ec296-111">We recommend using the new and improved, lightweight [notification SDK](https://aka.ms/GNSDK) instead of the cross-device [Project Rome SDK](https://github.com/microsoft/project-rome).</span></span>

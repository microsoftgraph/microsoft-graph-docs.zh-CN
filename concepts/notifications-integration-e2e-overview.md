---
title: '与 Microsoft Graph 通知集成 '
description: '通知是与应用程序用户再次交互的最有效的方式之一。 可以通过几个简单的步骤将应用程序与 Microsoft Graph 通知集成。  '
localization_priority: Priority
ms.prod: notifications
author: merzink
ms.openlocfilehash: 8dc5ef886106ca4d966e0a94ae2915040cfb5d1f1ea66d041d136db5bb7951e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149526"
---
# <a name="integrate-with-microsoft-graph-notifications"></a>与 Microsoft Graph 通知集成

可以通过几个简单的步骤（如下图所示）将应用程序与 Microsoft Graph 通知集成。

![显示载入通知步骤的图片：注册、跨设备载入、服务器集成和客户端集成](images/notifications-integration-e2e-overview.png)

1.  在 Microsoft Azure 门户中[注册](notifications-integration-app-registration.md)应用程序。

2. [载入](notifications-integration-cross-device-experiences-onboarding.md)到合作伙伴中心/Windows 开发人员中心，以获取 Windows、iOS 和 Android 的跨平台应用程序标识和推送通知凭据。

3.  [将应用程序服务器](notifications-integrating-app-server.md)设置为通过 Microsoft Graph 发送通知。

4.  [将](notifications-integrating-with-windows.md)新的[通知客户端 SDK](https://aka.ms/GNSDK) 集成到 Windows、iOS、Android 或 Web 客户端，以接收和管理通知。

> [!NOTE]
> 我们建议使用新增和改进的轻型[通知 SDK](https://aka.ms/GNSDK)，而不是跨设备 [Project Rome SDK](https://github.com/microsoft/project-rome)。

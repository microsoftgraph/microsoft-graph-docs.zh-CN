---
title: '与 Microsoft Graph 通知集成 '
description: '通知是与应用程序用户再次交互的最有效的方式之一。 可以通过几个简单的步骤将应用程序与 Microsoft Graph 通知集成。  '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: 2f3a126ade92ff1615848f9f4db846aebb62d5f7
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063260"
---
# <a name="integrate-with-microsoft-graph-notifications"></a>与 Microsoft Graph 通知集成

可以通过几个简单的步骤（如下图所示）将应用程序与 Microsoft Graph 通知集成。

![显示载入通知步骤的图片：注册、跨设备载入、服务器集成和客户端集成](images/notifications-integration-e2e-overview.png)

1.  在 Microsoft Azure 门户中[注册](notifications-integration-app-registration.md)应用程序。

2.  [载入](notifications-integration-cross-device-experiences-onboarding.md)到合作伙伴中心/Windows 开发人员中心，以获取跨平台应用程序标识和推送通知凭据。

3.  [将应用程序服务器](notifications-integrating-app-server.md)设置为通过 Microsoft Graph 发送通知。

4.  [将](notifications-integrating-with-windows.md) [Microsoft Graph 通知客户端 SDK](https://github.com/microsoft/project-rome) 集成到 Windows、Android 或 iOS 应用程序客户端，以接收和管理通知。

---
title: windowsPrivacyDataCategory 枚举类型
description: 隐私数据访问的 Windows 隐私数据类别说明符。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 03a7e1d7f017d7c7df9c27257c8f2a3e01c861d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931186"
---
# <a name="windowsprivacydatacategory-enum-type"></a>windowsPrivacyDataCategory 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

隐私数据访问的 Windows 隐私数据类别说明符。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|指定无访问级别，没有方法。 设备可能表现，可以如 UserInControl 或 ForceAllow 中所示。 它可能依赖的隐私数据已访问它们，Windows 版本和其他因素。|
|accountInfo|1|允许应用程序访问用户的名称、 图片和中的 Microsoft 帐户创建其他帐户信息。 已添加到 Windows 10 版本 1607 中。|
|appsRunInBackground|2|允许应用程序接收的信息，请发送通知，并保持最新的即使用户未使用它们。 注意从背景 access 禁用 （电子邮件、 语音等） 的通信应用程序时这些应用程序可能也可能无法正常，因为它们是具有背景访问权限。 添加 Windows 10，版本 1703年中。|
|日历|3|允许应用程序访问用户的日历。 已添加到 Windows 10 版本 1607 中。|
|callHistory|4|允许应用程序访问用户的呼叫历史记录。 已添加到 Windows 10 版本 1607 中。|
|摄像机|5|允许应用程序访问用户的设备上的摄像头。 已添加到 Windows 10 版本 1607 中。|
|contacts|6|允许应用程序访问用户的联系人信息。 已添加到 Windows 10 版本 1607 中。|
|diagnosticsInfo|7|允许应用程序访问其他运行的应用程序的诊断信息。 添加 Windows 10，版本 1703年中。|
|email|8|允许应用程序访问并发送电子邮件。 已添加到 Windows 10 版本 1607 中。|
|location|9|允许访问设备用户的精确位置数据的应用程序。 已添加到 Windows 10 版本 1607 中。|
|消息|10|允许应用程序读取或发送邮件、 文本或 MMS。 已添加到 Windows 10 版本 1607 中。|
|microphone|11|让用户设备上使用麦克风的应用程序。 已添加到 Windows 10 版本 1607 中。|
|动态|12|允许使用动态数据在设备用户生成的应用程序。 已添加到 Windows 10 版本 1607 中。|
|通知|13|允许应用程序访问用户的通知。 已添加到 Windows 10 版本 1607 中。|
|phone|14|允许应用程序访问电话数据和发起电话呼叫。 已添加到 Windows 10 版本 1607 中。|
|无线电|15|让无线电，包括蓝牙，用于发送和接收这些数据的应用程序。 已添加到 Windows 10 版本 1607 中。|
|tasks|16|允许应用程序访问任务计划程序。 添加 Windows 10，版本 1703年中。|
|syncWithDevices|17|允许应用程序自动共享，并且不明确配对与用户的设备的无线设备同步信息。 已添加到 Windows 10 版本 1607 中。|
|trustedDevices|18|允许应用程序访问受信任的设备。 已添加到 Windows 10 版本 1607 中。|






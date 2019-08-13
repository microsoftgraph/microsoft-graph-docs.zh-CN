---
title: windowsPrivacyDataCategory 枚举类型
description: 用于隐私数据访问的 Windows 隐私数据类别说明符。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 60f1e417b937a629f9069e81e51f64cff508f71f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369638"
---
# <a name="windowsprivacydatacategory-enum-type"></a>windowsPrivacyDataCategory 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于隐私数据访问的 Windows 隐私数据类别说明符。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未指定访问级别, 无意向。 在 UserInControl 或 ForceAllow 中, 设备的行为可能是一样的。 它可能取决于访问的隐私数据、Windows 版本和其他因素。|
|accountInfo|1|允许应用访问用户的名称、图片以及在 Microsoft 帐户中创建的其他帐户信息。 已添加到 Windows 10 版本 1607 中。|
|appsRunInBackground|双面|允许应用接收信息、发送通知并保持最新状态, 即使用户不使用它们也是如此。 请注意, 从后台访问禁用通信应用程序 (电子邮件、语音等) 时, 这些应用程序可能会也可能不会像背景访问中那样正常工作。 在 Windows 10 版本1703中添加。|
|calendar|第三章|允许应用访问用户的日历。 已添加到 Windows 10 版本 1607 中。|
|callHistory|4|允许应用访问用户的呼叫历史记录。 已添加到 Windows 10 版本 1607 中。|
|拍照|5|允许应用访问用户设备上的摄像头。 已添加到 Windows 10 版本 1607 中。|
|contacts|型|允许应用访问用户的联系信息。 已添加到 Windows 10 版本 1607 中。|
|diagnosticsInfo|步|允许应用访问其他正在运行的应用程序的诊断信息。 在 Windows 10 版本1703中添加。|
|email|utf-8|允许应用访问和发送电子邮件。 已添加到 Windows 10 版本 1607 中。|
|location|第|允许应用访问设备用户的确切位置数据。 已添加到 Windows 10 版本 1607 中。|
|讯息|10 |允许应用读取或发送消息、文本或 MMS。 已添加到 Windows 10 版本 1607 中。|
|着|11x17|允许应用在用户设备上使用麦克风。 已添加到 Windows 10 版本 1607 中。|
|动作|12|允许应用使用在设备用户上生成的运动数据。 已添加到 Windows 10 版本 1607 中。|
|通知|13|允许应用访问用户的通知。 已添加到 Windows 10 版本 1607 中。|
|phone|日|允许应用访问电话数据并拨打电话。 已添加到 Windows 10 版本 1607 中。|
|收发|个|允许应用使用无线收发器 (包括蓝牙) 发送和接收数据。 已添加到 Windows 10 版本 1607 中。|
|tasks|位|允许应用访问任务计划程序。 在 Windows 10 版本1703中添加。|
|syncWithDevices|×|允许应用自动与未明确配对用户设备的无线设备共享和同步信息。 已添加到 Windows 10 版本 1607 中。|
|trustedDevices|18|允许应用访问受信任的设备。 已添加到 Windows 10 版本 1607 中。|




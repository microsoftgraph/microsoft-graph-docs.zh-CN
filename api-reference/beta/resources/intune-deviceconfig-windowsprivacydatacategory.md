---
title: windowsPrivacyDataCategory 枚举类型
description: Windows隐私数据访问的隐私数据类别说明。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1883e1518526945def0ae8bbd982fa71276c68a0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59105900"
---
# <a name="windowsprivacydatacategory-enum-type"></a>windowsPrivacyDataCategory 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows隐私数据访问的隐私数据类别说明。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未指定访问级别，没有意图。 设备的行为类似于 UserInControl 或 ForceAllow。 它可能取决于已访问的隐私数据、Windows版本和其他因素。|
|accountInfo|1|允许应用访问在 Microsoft 帐户中创建的用户名、图片和其他帐户信息。 已添加到 Windows 10 版本 1607 中。|
|appsRunInBackground|2|允许应用接收信息、发送通知和保持最新，即使用户没有使用它们。 请注意，当从后台访问 (电子邮件、) 等通信应用时，这些应用可以或可能不会像后台访问一样运行。 已添加到Windows 10版本 1703 中。|
|日历|3|允许应用访问用户的日历。 已添加到 Windows 10 版本 1607 中。|
|callHistory|4 |允许应用访问用户的呼叫历史记录。 已添加到 Windows 10 版本 1607 中。|
|相机|5 |允许应用访问用户设备上相机。 已添加到 Windows 10 版本 1607 中。|
|contacts|6 |允许应用访问用户的联系人信息。 已添加到 Windows 10 版本 1607 中。|
|diagnosticsInfo|7 |允许应用访问有关其他正在运行的应用的诊断信息。 已添加到Windows 10版本 1703 中。|
|email|8 |允许应用访问和发送电子邮件。 已添加到 Windows 10 版本 1607 中。|
|位置|9 |允许应用访问设备用户的确切位置数据。 已添加到 Windows 10 版本 1607 中。|
|消息传递|10 |允许应用读取或发送消息、文本或彩信。 已添加到 Windows 10 版本 1607 中。|
|麦克风|11|允许应用在用户设备上使用麦克风。 已添加到 Windows 10 版本 1607 中。|
|动作|12 |让应用使用在设备用户上生成的运动数据。 已添加到 Windows 10 版本 1607 中。|
|通知|13|允许应用访问用户通知。 已添加到 Windows 10 版本 1607 中。|
|phone|14 |允许应用访问电话数据和进行电话呼叫。 已添加到 Windows 10 版本 1607 中。|
|无线电广播|15 |允许应用使用无线电设备（蓝牙）发送和接收数据。 已添加到 Windows 10 版本 1607 中。|
|tasks|16 |允许应用访问任务计划程序。 已添加到Windows 10版本 1703 中。|
|syncWithDevices|17 |让应用自动与未与用户设备显式配对的无线设备共享和同步信息。 已添加到 Windows 10 版本 1607 中。|
|trustedDevices|18 |允许应用访问受信任的设备。 已添加到 Windows 10 版本 1607 中。|




---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许该设备发送诊断和使用情况的遥测数据，如 Watson。
localization_priority: Normal
ms.openlocfilehash: 1654e9c5c94fd79bbda0d77ef84101fb9fb92d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812780"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

允许该设备发送诊断和使用情况的遥测数据，如 Watson。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|用户定制|0|允许用户设置。|
|无|1|从操作系统组件不发送任何遥测数据。 注意： 此值才适用于企业和服务器设备。 在其他设备上使用此设置等同于设置 1 的值。|
|基本|2|发送基本遥测数据。|
|增强|3|发送增强，包括使用情况和见解数据的遥测数据。|
|完整|4|发送完全遥测数据，包括诊断数据，如系统状态。|




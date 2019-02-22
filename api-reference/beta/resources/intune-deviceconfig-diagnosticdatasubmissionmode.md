---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用遥测数据, 如 Watson。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e749d2fc7a1eb191c62fbc9db389887cdd901c27
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175218"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

允许设备发送诊断和使用遥测数据, 如 Watson。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|允许用户进行设置。|
|无|1|不会从 OS 组件发送遥测数据。 注意: 此值仅适用于企业和服务器设备。 在其他设备上使用此设置等效于将值设置为1。|
|vba|双面|发送基本遥测数据。|
|有所|第三章|发送包含使用率和见解数据的增强遥测数据。|
|全|4|发送包含诊断数据 (如系统状态) 的完整遥测数据。|





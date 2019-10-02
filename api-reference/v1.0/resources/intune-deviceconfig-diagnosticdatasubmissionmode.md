---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用遥测数据，如 Watson。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 15abccb0bf2171e62c2b468ecf5c3078e052ea75
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359374"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode 枚举类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

允许设备发送诊断和使用遥测数据，如 Watson。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|允许用户进行设置。|
|无|1|不会从 OS 组件发送遥测数据。 注意：此值仅适用于企业和服务器设备。 在其他设备上使用此设置等效于将值设置为1。|
|vba|双面|发送基本遥测数据。|
|有所|第三章|发送包含使用率和见解数据的增强遥测数据。|
|全|4|发送包含诊断数据（如系统状态）的完整遥测数据。|





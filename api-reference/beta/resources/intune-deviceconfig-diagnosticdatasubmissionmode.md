---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许该设备发送诊断和使用情况的遥测数据，如 Watson。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b587d6872bcd3610c3b878ae7a672c3e776ea01
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422255"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

允许该设备发送诊断和使用情况的遥测数据，如 Watson。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|用户定制|0|允许用户设置。|
|无|1|从操作系统组件不发送任何遥测数据。 注意： 此值才适用于企业和服务器设备。 在其他设备上使用此设置等同于设置 1 的值。|
|基本|2|发送基本遥测数据。|
|增强|3|发送增强，包括使用情况和见解数据的遥测数据。|
|完整|4|发送完全遥测数据，包括诊断数据，如系统状态。|





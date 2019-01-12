---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8d725213790260ece51c02bb81f2394fc8602095
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917340"
---
# <a name="devicecomplianceactiontype-enum-type"></a>deviceComplianceActionType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

计划操作类型枚举
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|noAction|0|任何操作|
|通知|1|发送通知|
|阻止|2|阻止 AAD 中的设备|
|停用|3|停用设备|
|擦除|4|擦除设备|
|removeResourceAccessProfiles|5|从设备中删除资源访问配置文件|
|pushNotification|9|向设备发送推送通知|




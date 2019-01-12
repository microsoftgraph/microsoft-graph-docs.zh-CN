---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1856847cb8a8ecf48ee6d13067bd24515326d89
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973207"
---
# <a name="devicecomplianceactiontype-enum-type"></a>deviceComplianceActionType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

计划操作类型枚举
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noAction|0|任何操作|
|通知|1|发送通知|
|阻止|2|阻止 AAD 中的设备|
|停用|3|停用设备|
|擦除|4|擦除设备|
|removeResourceAccessProfiles|5|从设备中删除资源访问配置文件|
|pushNotification|9|向设备发送推送通知|
|remoteLock|10|远程锁定设备|






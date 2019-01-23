---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cd0db68a21fff79ddbab924e8a1d9bd2ff2e542d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425741"
---
# <a name="devicecomplianceactiontype-enum-type"></a>deviceComplianceActionType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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





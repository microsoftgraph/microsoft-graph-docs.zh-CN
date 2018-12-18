---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: tfitzmac
ms.openlocfilehash: 84bef94d7352c13b49f223b859cea218932f8cad
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328684"
---
# <a name="devicecomplianceactiontype-enum-type"></a>deviceComplianceActionType 枚举类型

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




---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b39ea3291658bf97f072e7e6243d6920a0e51e78549cc3527615cf40fd69b883
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146487"
---
# <a name="devicecomplianceactiontype-enum-type"></a>deviceComplianceActionType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计划操作类型枚举

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noAction|0|无操作|
|通知|1|发送通知|
|block|2|在 AAD 中阻止设备|
|retire|3|停用设备|
|wipe|4 |擦除设备|
|removeResourceAccessProfiles|5 |从设备中删除资源访问配置文件|
|pushNotification|9 |向设备发送推送通知|





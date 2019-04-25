---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd370f9e706955d76de519a518b4659ba46c6d25
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534309"
---
# <a name="devicecomplianceactiontype-enum-type"></a>deviceComplianceActionType 枚举类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计划操作类型枚举

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noAction|0|无操作|
|通告|1|发送通知|
|数据|2 |阻止 AAD 中的设备|
|注销|3 |停用设备|
|擦|4 |擦除设备|
|removeResourceAccessProfiles|5 |从设备中删除资源访问配置文件|
|pushNotification|9 |将推送通知发送到设备|




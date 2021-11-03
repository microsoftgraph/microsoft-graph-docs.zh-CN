---
title: deviceManagementComplianceActionType 枚举类型
description: 计划操作类型枚举
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 705390a1d26ff9d74f7a6b9bb678b77e723a9236
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688252"
---
# <a name="devicemanagementcomplianceactiontype-enum-type"></a>deviceManagementComplianceActionType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计划操作类型枚举

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noAction|0|无操作|
|通知|1|发送通知|
|block|2|阻止设备AAD|
|retire|3|停用设备|
|wipe|4 |擦除设备|
|removeResourceAccessProfiles|5|从设备中删除资源访问配置文件|
|pushNotification|9 |向设备发送推送通知|
|remoteLock|10 |远程锁定设备|




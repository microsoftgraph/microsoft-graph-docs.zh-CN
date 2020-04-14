---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f0a5a3b4ab73bc0d97b5b47619cdcabb401400f2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437390"
---
# <a name="devicecomplianceactiontype-enum-type"></a>deviceComplianceActionType 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计划操作类型枚举

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noAction|0|无操作|
|通告|1|发送通知|
|数据|双面|阻止 AAD 中的设备|
|注销|第三章|停用设备|
|擦|4 |擦除设备|
|removeResourceAccessProfiles|5 |从设备中删除资源访问配置文件|
|pushNotification|9 |将推送通知发送到设备|
|remoteLock|10 |远程锁定设备|




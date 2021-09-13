---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e7ab0dca825607b0ad3309dcd3cab138b875c418
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040454"
---
# <a name="devicecomplianceactiontype-enum-type"></a>deviceComplianceActionType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

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
|remoteLock|10 |远程锁定设备|




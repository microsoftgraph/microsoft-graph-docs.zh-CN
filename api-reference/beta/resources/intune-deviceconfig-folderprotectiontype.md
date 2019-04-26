---
title: folderProtectionType 枚举类型
description: 文件夹保护的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 741565678be1bfb533c4445c02c767f87fdfca05
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556086"
---
# <a name="folderprotectiontype-enum-type"></a>folderProtectionType 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

文件夹保护的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|设备默认值, 无意向。|
|启用|1|阻止功能。|
|auditMode|2 |允许功能, 但生成日志。|
|blockDiskModification|3 |阻止不受信任的应用写入磁盘扇区。|
|auditDiskModification|4 |在不受信任的应用写入磁盘扇区时生成日志。|






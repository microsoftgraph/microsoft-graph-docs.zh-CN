---
title: folderProtectionType 枚举类型
description: 文件夹保护的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d3116e2663a9217e19f32f4e1c6cbc068d856fd0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994942"
---
# <a name="folderprotectiontype-enum-type"></a>folderProtectionType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

文件夹保护的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|设备默认值, 无意向。|
|启用|1|阻止功能。|
|auditMode|双面|允许功能, 但生成日志。|
|blockDiskModification|第三章|阻止不受信任的应用写入磁盘扇区。|
|auditDiskModification|4|在不受信任的应用写入磁盘扇区时生成日志。|






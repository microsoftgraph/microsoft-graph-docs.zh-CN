---
title: folderProtectionType 枚举类型
description: 文件夹保护的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 23717d1e798059f1ca025a3f80279804b616b17f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529985"
---
# <a name="folderprotectiontype-enum-type"></a>folderProtectionType 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

文件夹保护的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|设备默认值，无意向。|
|启用|1 |阻止功能。|
|auditMode|2 |允许功能，但生成日志。|
|blockDiskModification|3 |阻止不受信任的应用写入磁盘扇区。|
|auditDiskModification|4 |在不受信任的应用写入磁盘扇区时生成日志。|




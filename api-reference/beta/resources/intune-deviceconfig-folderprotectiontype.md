---
title: folderProtectionType 枚举类型
description: 文件夹保护的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a8242f361f68ec7e295950ea29e7478de414ad6b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791735"
---
# <a name="folderprotectiontype-enum-type"></a>folderProtectionType 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

文件夹保护的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|设备默认值，无意向。|
|启用|1|阻止功能。|
|auditMode|双面|允许功能，但生成日志。|
|blockDiskModification|第三章|阻止不受信任的应用写入磁盘扇区。|
|auditDiskModification|4 |在不受信任的应用写入磁盘扇区时生成日志。|




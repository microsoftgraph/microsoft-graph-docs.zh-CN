---
title: folderProtectionType 枚举类型
description: 文件夹保护的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e0a368486f7fa8e1d869e7cc870fdfdca34c75a96eca216008b27ea36ed0eaa0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54203111"
---
# <a name="folderprotectiontype-enum-type"></a>folderProtectionType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

文件夹保护的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|设备默认值，无意图。|
|enable|1 |阻止功能。|
|auditMode|2 |允许功能，但生成日志。|
|blockDiskModification|3 |阻止不受信任的应用写入磁盘扇区。|
|auditDiskModification|4 |当不受信任的应用写入磁盘扇区时生成日志。|





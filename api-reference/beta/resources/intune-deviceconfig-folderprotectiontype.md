---
title: folderProtectionType 枚举类型
description: 可能的值的文件夹保护
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 435f3ea01f5a8ffc3c4cb54034d415d54732db5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826129"
---
# <a name="folderprotectiontype-enum-type"></a>folderProtectionType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

可能的值的文件夹保护
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|用户定制|0|设备默认值，没有用途。|
|启用|1|阻止功能。|
|auditMode|2|允许功能，但生成日志。|
|blockDiskModification|3|阻止来自写入磁盘扇区的不受信任应用程序。|
|auditDiskModification|4|时不受信任应用程序写入磁盘扇区生成日志。|






---
title: folderProtectionType 枚举类型
description: 可能的值的文件夹保护
ms.openlocfilehash: a02f1602f8b9a962124fb7bf2a9731662a6f3057
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044352"
---
# <a name="folderprotectiontype-enum-type"></a>folderProtectionType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

可能的值的文件夹保护
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|用户定制|0|设备默认值，没有用途。|
|启用|1|阻止功能。|
|auditMode|2|允许功能，但生成日志。|
|blockDiskModification|3|阻止来自写入磁盘扇区的不受信任应用程序。|
|auditDiskModification|4|时不受信任应用程序写入磁盘扇区生成日志。|






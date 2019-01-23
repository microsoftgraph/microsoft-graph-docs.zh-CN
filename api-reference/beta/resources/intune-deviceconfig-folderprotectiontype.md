---
title: folderProtectionType 枚举类型
description: 可能的值的文件夹保护
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e2abbb719ab93b53ad276f8391d4028c4f8b40b4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405714"
---
# <a name="folderprotectiontype-enum-type"></a>folderProtectionType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

可能的值的文件夹保护

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|用户定制|0|设备默认值，没有用途。|
|启用|1|阻止功能。|
|auditMode|2|允许功能，但生成日志。|
|blockDiskModification|3|阻止来自写入磁盘扇区的不受信任应用程序。|
|auditDiskModification|4|时不受信任应用程序写入磁盘扇区生成日志。|





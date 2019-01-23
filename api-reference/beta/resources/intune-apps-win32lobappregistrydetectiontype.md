---
title: win32LobAppRegistryDetectionType 枚举类型
description: 包含所有支持的注册表数据检测类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 188f206e42b55e0c2cc2f8b6ed831f19a4b2052a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411083"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a>win32LobAppRegistryDetectionType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含所有支持的注册表数据检测类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置。|
|存在|1|指定的注册表项或值存在。|
|doesNotExist|2|指定的注册表项的值不存在。|
|string|3|字符串值类型。|
|integer|4|整数值类型。|
|version|5|版本值类型。|





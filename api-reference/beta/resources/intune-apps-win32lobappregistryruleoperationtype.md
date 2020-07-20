---
title: win32LobAppRegistryRuleOperationType 枚举类型
description: 包含所有受支持的注册表数据检测类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b0aefbf5fd234bac0704c9c9f983e19ed11cbcfe
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790304"
---
# <a name="win32lobappregistryruleoperationtype-enum-type"></a>win32LobAppRegistryRuleOperationType 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含所有受支持的注册表数据检测类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置。|
|存在|1 |指定的注册表项或值存在。|
|doesNotExist|双面|指定的注册表项或值不存在。|
|string|第三章|字符串值类型。|
|integer|4 |整型值类型。|
|version|5 |版本值类型。|




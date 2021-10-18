---
title: win32LobAppRegistryRuleOperationType 枚举类型
description: 包含所有支持的注册表数据检测类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 230ed063b4b0aee33a52f27e48ade03e65f02df8
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60448609"
---
# <a name="win32lobappregistryruleoperationtype-enum-type"></a>win32LobAppRegistryRuleOperationType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含所有支持的注册表数据检测类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置。|
|exists|1|指定的注册表项或值已存在。|
|doesNotExist|2|指定的注册表项或值不存在。|
|string|3|字符串值类型。|
|integer|4 |整数值类型。|
|version|5|版本值类型。|




---
title: win32LobAppRegistryRuleOperationType 枚举类型
description: 包含所有支持的注册表数据检测类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 55b02e66f9735bc28ad0ec17bafc0ec5f549b7f1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59015600"
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
|字符串|3|字符串值类型。|
|integer|4 |整数值类型。|
|version|5 |版本值类型。|





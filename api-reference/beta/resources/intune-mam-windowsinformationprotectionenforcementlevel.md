---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护强制级别的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 46488043220297617dfc4eb807d94ef2a9c0ba19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527835"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a>windowsInformationProtectionEnforcementLevel 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

WIP 保护强制级别的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noProtection|0|无保护强制实施|
|encryptAndAuditOnly|1 |仅加密和审核|
|encryptAuditAndPrompt|2 |加密、审核和提示|
|encryptAuditAndBlock|3 |加密、审核和阻止|




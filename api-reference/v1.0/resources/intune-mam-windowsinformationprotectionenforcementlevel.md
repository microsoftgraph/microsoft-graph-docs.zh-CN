---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护强制级别的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1901059ef45141b0dc40d91dcbf4d9237cd6fc5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561171"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a>windowsInformationProtectionEnforcementLevel 枚举类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

WIP 保护强制级别的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noProtection|0|无保护强制实施|
|encryptAndAuditOnly|1|仅加密和审核|
|encryptAuditAndPrompt|2 |加密、审核和提示|
|encryptAuditAndBlock|3 |加密、审核和阻止|




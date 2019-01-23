---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护实施级别的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 37ec9c781ea4a804260f7dff7b6586c042dcad48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417670"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a>windowsInformationProtectionEnforcementLevel 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

WIP 保护实施级别的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noProtection|0|无保护强制|
|encryptAndAuditOnly|1|加密和仅用于审核|
|encryptAuditAndPrompt|2|加密、 审核和提示|
|encryptAuditAndBlock|3|加密、 审核和阻止|





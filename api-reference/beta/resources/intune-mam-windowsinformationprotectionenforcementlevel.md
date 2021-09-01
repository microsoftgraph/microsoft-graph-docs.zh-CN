---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护强制级别的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d44fc165eb5c1a728e61c5b9a07ebc8f00a131de
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789245"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a>windowsInformationProtectionEnforcementLevel 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

WIP 保护强制级别的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noProtection|0|不强制执行保护|
|encryptAndAuditOnly|1|仅加密和审核|
|encryptAuditAndPrompt|2|加密、审核和提示|
|encryptAuditAndBlock|3|加密、审核和阻止|




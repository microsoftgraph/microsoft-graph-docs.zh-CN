---
title: endpointSecurityConfigurationProfileType 枚举类型
description: 终结点安全策略配置文件类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e766ad484d26abd770e2655b1f75e455306ad82
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793232"
---
# <a name="endpointsecurityconfigurationprofiletype-enum-type"></a>endpointSecurityConfigurationProfileType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

终结点安全策略配置文件类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|陌生.|
|程序|1|程序.|
|windowsSecurity|双面|Windows 安全性。|
|bitLocker|第三章|BitLocker.|
|fileVault|4 |FileVault.|
|firewall|5 |Firewall.|
|firewallRules|6 |防火墙规则。|
|endpointDetectionAndResponse|7 |终结点检测和响应。|
|deviceControl|8 |设备控件。|
|appAndBrowserIsolation|9 |应用程序和浏览器隔离。|
|exploitProtection|10 |Exploit Protection。|
|webProtection|11x17|Web 保护。|
|applicationControl|12 |应用程序控制。|
|attackSurfaceReductionRules|13|攻击面减少规则。|
|accountProtection|14 |帐户保护。|




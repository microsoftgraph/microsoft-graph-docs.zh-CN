---
title: deviceManagementConfigurationTemplateFamily 枚举类型
description: 描述 Template 实体的 TemplateFamily
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 91d79cde2cb07f63dd039fac07c09f56399bc11b
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60486985"
---
# <a name="devicemanagementconfigurationtemplatefamily-enum-type"></a>deviceManagementConfigurationTemplateFamily 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述 Template 实体的 TemplateFamily

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|策略未链接到模板时，模板系列默认为|
|endpointSecurityAntivirus|10 |EndpointSecurity 防病毒的模板系列，用于管理托管设备的离散防病毒设置组|
|endpointSecurityDiskEncryption|11|EndpointSecurityDiskEncryption 的模板系列，提供与设备内置加密方法（如 FileVault 或 BitLocker）相关的设置|
|endpointSecurityFirewall|12 |EndpointSecurityFirewall 的模板系列，可帮助为运行 macOS 和 Windows 10|
|endpointSecurityEndpointDetectionAndResponse|13|EndpointSecurityEndpointDetectionAndResponse 的模板系列，便于管理 EDR 设置，将设备载入 Microsoft Defender for Endpoint|
|endpointSecurityAttackSurfaceReduction|14 |EndpointSecurityAttackSurfaceReduction 的模板系列，通过最大程度地减少组织易受网络威胁和攻击的位置，帮助减少攻击面|
|endpointSecurityAccountProtection|15 |EndpointSecurityAccountProtection 的模板系列，有助于保护用户的标识和帐户|
|endpointSecurityApplicationControl|16|ApplicationControl 的模板系列，通过限制用户可运行的应用程序以及 System Core 中运行的代码和内核 (缓解) |
|比较基准|20|基线的模板系列|




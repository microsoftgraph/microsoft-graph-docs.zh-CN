---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a157111db947e9e7c186c30be6cc63a709b82922
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671668"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType 枚举类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理代理类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|大通|1|设备由 Exchange 服务器管理。|
|Mdm|2|设备由 Intune MDM 管理。|
|easMdm|3|设备由 Exchange 服务器和 Intune MDM 管理。|
|intuneClient|4|Intune客户端托管。|
|easIntuneClient|5|设备是 EAS，Intune客户端双重托管。|
|configurationManagerClient|8 |设备由Configuration Manager管理。|
|configurationManagerClientMdm|10|设备由Configuration Manager和 MDM 管理。|
|configurationManagerClientMdmEas|11|设备由 Configuration Manager、MDM 和 Eas 管理。|
|unknown|16|未知的管理代理类型。|
|jamf|32|设备属性是从 Jamf 提取的。|
|googleCloudDevicePolicyController|64|该设备由 Google 的 CloudDPC 管理。|
|microsoft365ManagedMdm|258|此设备由 Microsoft 365 通过Intune管理。|
|msSense|1024|尚未记录|
|intuneAosp|2048|此设备由 Intune 的适用于 AOSP 的 MDM (Android 开源项目) 设备管理|





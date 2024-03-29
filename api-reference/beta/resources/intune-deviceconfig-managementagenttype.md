---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: afda1f2dd54cbb0ee63dc47e3ca14bf6cd946a1b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086769"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理代理类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|eas|1|设备由Exchange管理。|
|mdm|2|设备由 Intune MDM 管理。|
|easMdm|3|设备由 Exchange 和 Intune MDM 管理。|
|intuneClient|4 |Intune 客户端托管。|
|easIntuneClient|5 |设备是 EAS 和 Intune 客户端双托管设备。|
|configurationManagerClient|8 |设备由 Configuration Manager 管理。|
|configurationManagerClientMdm|10 |设备由 Configuration Manager 和 MDM 管理。|
|configurationManagerClientMdmEas|11|设备由 Configuration Manager、MDM 和 Eas 管理。|
|unknown|16 |未知管理代理类型。|
|jamf|32|设备属性从 Jamf 获取。|
|googleCloudDevicePolicyController|64|设备由 Google 的 CloudDPC 管理。|
|microsoft365ManagedMdm|258|此设备通过 Intune Microsoft 365管理。|
|windowsManagementCloudApi|512|此设备由 Windows云 API 管理。|




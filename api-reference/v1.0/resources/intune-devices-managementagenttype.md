---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9743c9c83e34a0c58dee78e73839f8fdcaaf2cda
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251564"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType 枚举类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理代理类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|符合|1|设备由 Exchange server 管理。|
|mdm|双面|设备由 Intune MDM 管理。|
|easMdm|第三章|设备由 Exchange server 和 Intune MDM 管理。|
|intuneClient|4|Intune 客户端托管。|
|easIntuneClient|5|设备为 EAS 和 Intune 客户端双重托管。|
|configurationManagerClient|utf-8|设备由配置管理器管理。|
|configurationManagerClientMdm|10|设备由 Configuration Manager 和 MDM 管理。|
|configurationManagerClientMdmEas|11x17|设备由 Configuration Manager、MDM 和 Eas 管理。|
|unknown|位|未知的管理代理类型。|
|jamf|32|设备属性是从 Jamf 中提取的。|
|googleCloudDevicePolicyController|64|设备由 Google 的 CloudDPC 管理。|




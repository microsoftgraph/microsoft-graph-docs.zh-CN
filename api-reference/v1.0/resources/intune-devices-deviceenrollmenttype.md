---
title: deviceEnrollmentType 枚举类型
description: 将移动设备添加到管理中的可能方法。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0ac6112e63511a79ac5a64f14e916b497a949db0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755238"
---
# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

将移动设备添加到管理中的可能方法。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值，未收集注册类型。|
|userEnrollment|1|用户通过 BYOD 渠道推动注册。|
|deviceEnrollmentManager|2|使用设备注册管理器帐户的用户注册。|
|appleBulkWithUser|3|具有用户质询的 Apple 批量注册。  (DEP、Apple Configurator) |
|appleBulkWithoutUser|4 |Apple 批量注册，无需用户质询。  (DEP、Apple Configurator、Mobile Config) |
|windowsAzureADJoin|5 |Windows 10加入 Azure AD。|
|windowsBulkUserless|6 |Windows 10使用证书通过 ICD 批量注册。|
|windowsAutoEnrollment|7 |Windows 10自动注册。  (添加工作帐户) |
|windowsBulkAzureDomainJoin|8 |Windows 10 Azure AD 批量加入。|
|windowsCoManagement|9 |Windows 10 Co-Management AutoPilot 或组策略触发。|
|windowsAzureADJoinUsingDeviceAuth|10  |Windows 10使用设备身份验证加入 Azure AD。|
|appleUserEnrollment|11|由 Apple 用户注册管理的设备|
|appleUserEnrollmentWithServiceAccount|12 |使用服务帐户由 Apple 用户注册管理的设备|





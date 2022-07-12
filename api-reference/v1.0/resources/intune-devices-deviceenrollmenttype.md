---
title: deviceEnrollmentType 枚举类型
description: 向管理添加移动设备的可能方法。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a53c4fadbce9703e4e68b54a86cfff80e1bd3944
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735367"
---
# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

向管理添加移动设备的可能方法。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值，未收集注册类型。|
|userEnrollment|1|通过 BYOD 通道进行用户驱动的注册。|
|deviceEnrollmentManager|2|使用设备注册管理器帐户进行用户注册。|
|appleBulkWithUser|3|具有用户质询的 Apple 批量注册。  (DEP，Apple Configurator) |
|appleBulkWithoutUser|4|无需用户质询的 Apple 批量注册。  (DEP、Apple Configurator、Mobile Config) |
|windowsAzureADJoin|5|Windows 10 Azure AD 联接。|
|windowsBulkUserless|6 |使用证书通过 ICD Windows 10批量注册。|
|windowsAutoEnrollment|7 |Windows 10自动注册。  (添加工作帐户) |
|windowsBulkAzureDomainJoin|8 |Windows 10批量 Azure AD 联接。|
|windowsCoManagement|9 |由 AutoPilot 或 نهج المجموعة 触发的Windows 10 Co-Management。|
|windowsAzureADJoinUsingDeviceAuth|10|使用设备身份验证Windows 10 Azure AD 联接。|
|appleUserEnrollment|11|由 Apple 用户注册管理的设备|
|appleUserEnrollmentWithServiceAccount|12 |使用服务帐户由 Apple 用户注册管理的设备|






---
title: deviceEnrollmentType 枚举类型
description: 将移动设备添加到管理中的可能方法。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4f0e309126d48646fb67446270353566be23ec9a
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732360"
---
# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

将移动设备添加到管理中的可能方法。

## <a name="members"></a>成员
|成员|值|Description|
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










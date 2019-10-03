---
title: deviceEnrollmentType 枚举类型
description: 向管理层添加移动设备的可能方法。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ae60fd6657cf902eb5bdd0f919d446527b00d9a9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368272"
---
# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 枚举类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

向管理层添加移动设备的可能方法。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值，未收集注册类型。|
|userEnrollment|1|通过 BYOD 通道的用户驱动的注册。|
|deviceEnrollmentManager|双面|具有设备注册管理员帐户的用户注册。|
|appleBulkWithUser|第三章|使用用户质询的 Apple 批量注册。 （DEP、Apple 配置器）|
|appleBulkWithoutUser|4|没有用户质询的 Apple 批量注册。 （DEP、Apple 配置器、移动配置）|
|windowsAzureADJoin|5|Windows 10 Azure AD 加入。|
|windowsBulkUserless|型|通过带证书的 ICD 通过 ICD 进行的 Windows 10 批量注册。|
|windowsAutoEnrollment|步|Windows 10 自动注册。 （添加工作帐户）|
|windowsBulkAzureDomainJoin|utf-8|Windows 10 批量 Azure AD 加入。|
|windowsCoManagement|第|由 AutoPilot 或组策略触发的 Windows 10 协同管理。|





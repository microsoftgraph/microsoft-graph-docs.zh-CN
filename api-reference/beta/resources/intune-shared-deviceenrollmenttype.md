---
title: deviceEnrollmentType 枚举类型
description: 将移动设备添加到管理的可能方式。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aed1f40604a765b1a434bca35dbb356e65e8ccd5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399288"
---
# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

将移动设备添加到管理的可能方式。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值，注册类型不是收集的。|
|userEnrollment|1|通过 BYOD 通道用户驱动的注册。|
|deviceEnrollmentManager|2|用户注册使用设备注册管理器帐户。|
|appleBulkWithUser|3|与用户质询 Apple 批量注册。 (DEP，Apple 配置器)|
|appleBulkWithoutUser|4|没有用户质询 Apple 批量注册。 （DEP，Apple 配置器移动配置）|
|windowsAzureADJoin|5|Windows Azure AD 10 加入。|
|windowsBulkUserless|6|Windows 10 批量注册通过 ICD 证书。|
|windowsAutoEnrollment|7|Windows 10 自动注册。 （添加工作帐户）|
|windowsBulkAzureDomainJoin|8|Windows 10 批量 Azure AD 加入。|
|windowsCoManagement|9|由自动执行某些操作或组策略触发 Windows 10 共同管理。|





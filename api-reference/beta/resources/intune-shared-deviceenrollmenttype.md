---
title: deviceEnrollmentType 枚举类型
description: 将移动设备添加到管理中的可能方法。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3d3bc9b0862dd376b393019838980ce9c82c7df3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440169"
---
# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 枚举类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

将移动设备添加到管理中的可能方法。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值，未收集注册类型。|
|userEnrollment|1 |用户通过 BYOD 渠道推动注册。|
|deviceEnrollmentManager|2 |使用设备注册管理器帐户的用户注册。|
|appleBulkWithUser|3 |具有用户质询的 Apple 批量注册。  (DEP、Apple Configurator) |
|appleBulkWithoutUser|4 |Apple 批量注册，无需用户质询。  (DEP、Apple Configurator、Mobile Config) |
|windowsAzureADJoin|5 |Windows 10 Azure AD 加入。|
|windowsBulkUserless|6 |Windows 10 使用证书通过 ICD 批量注册。|
|windowsAutoEnrollment|7 |Windows 10 自动注册。  (添加工作帐户) |
|windowsBulkAzureDomainJoin|8 |Windows 10 批量 Azure AD 加入。|
|windowsCoManagement|9 |Windows 10 Co-Management AutoPilot 或组策略触发。|
|windowsAzureADJoinUsingDeviceAuth|10  |使用设备身份验证加入 Windows 10 Azure AD。|
|appleUserEnrollment|11|由 Apple 用户注册管理的设备|
|appleUserEnrollmentWithServiceAccount|12 |由 Apple 用户使用服务帐户注册管理的设备|
|azureAdJoinUsingAzureVmExtension|14 |预配 Azure VM 时进行 Azure AD 加入注册|
|androidEnterpriseDedicatedDevice|15 |Android 企业专用设备|
|androidEnterpriseFullyManaged|16 |Android 企业版完全托管|
|androidEnterpriseCorporateWorkProfile|17 |Android 企业版企业工作配置文件|





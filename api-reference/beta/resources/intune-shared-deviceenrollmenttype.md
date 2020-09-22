---
title: deviceEnrollmentType 枚举类型
description: 向管理层添加移动设备的可能方法。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3242018f288e47104e6b668beeeb5d4eb3c53964
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055322"
---
# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

向管理层添加移动设备的可能方法。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值，未收集注册类型。|
|userEnrollment|1 |通过 BYOD 通道的用户驱动的注册。|
|deviceEnrollmentManager|2 |具有设备注册管理员帐户的用户注册。|
|appleBulkWithUser|第三章|使用用户质询的 Apple 批量注册。  (DEP、Apple 配置器) |
|appleBulkWithoutUser|4 |没有用户质询的 Apple 批量注册。  (DEP、Apple 配置器、移动配置) |
|windowsAzureADJoin|5 |Windows 10 Azure AD 加入。|
|windowsBulkUserless|6 |通过带证书的 ICD 通过 ICD 进行的 Windows 10 批量注册。|
|windowsAutoEnrollment|7 |Windows 10 自动注册。  (添加工作帐户) |
|windowsBulkAzureDomainJoin|8 |Windows 10 批量 Azure AD 加入。|
|windowsCoManagement|9 |由 AutoPilot 或组策略触发的 Windows 10 协同管理。|
|appleUserEnrollment|11 |由 Apple 用户注册管理的设备|
|appleUserEnrollmentWithServiceAccount|12 |由 Apple 用户使用服务帐户进行注册管理的设备|
|azureAdJoinUsingAzureVmExtension|14 |预配 Azure VM 时的 azure AD 加入注册|
|androidEnterpriseDedicatedDevice|15 |Android 企业专用设备|
|androidEnterpriseFullyManaged|16 |完全管理的 Android 企业版|
|androidEnterpriseCorporateWorkProfile|17 |Android 企业公司工作配置文件|







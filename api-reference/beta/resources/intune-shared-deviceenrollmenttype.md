---
title: deviceEnrollmentType 枚举类型
description: 将移动设备添加到管理的可能方式。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bffe0e592240cbeee22a63dac8c339a0d3b3ff3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946836"
---
# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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






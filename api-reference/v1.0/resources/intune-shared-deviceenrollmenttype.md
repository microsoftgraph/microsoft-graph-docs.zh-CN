---
title: deviceEnrollmentType 枚举类型
description: 将移动设备添加到管理的可能方式。
author: tfitzmac
ms.openlocfilehash: 88135947f882433a35fa518b750274f38f48dcc1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329601"
---
# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

将移动设备添加到管理的可能方式。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值，注册类型不是收集的。|
|userEnrollment|1|通过 BYOD 通道用户驱动的注册。|
|deviceEnrollmentManager|2|用户注册使用设备注册管理器帐户。|
|appleBulkWithUser|3|Apple 批量注册及用户质询 （DEP、 Apple 配置器）。|
|appleBulkWithoutUser|4|Apple 批量注册没有用户质询 （DEP，Apple 配置器 Mobile 配置）。|
|windowsAzureADJoin|5|Windows Azure AD 10 加入。|
|windowsBulkUserless|6|Windows 10 批量注册通过 ICD 证书。|
|windowsAutoEnrollment|7|Windows 10 自动注册。 （添加工作帐户）|
|windowsBulkAzureDomainJoin|8|Windows 10 批量 Azure AD 加入。|
|windowsCoManagement|9|Windows 10 共同管理触发自动执行某些操作或组策略。|




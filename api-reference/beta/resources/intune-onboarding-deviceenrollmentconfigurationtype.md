---
title: deviceEnrollmentConfigurationType 枚举类型
description: 介绍模板实体的 TemplateFamily
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 98fef8c27ca10a613c02132a4cd80fb8ab909205
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211317"
---
# <a name="deviceenrollmentconfigurationtype-enum-type"></a>deviceEnrollmentConfigurationType 枚举类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

介绍模板实体的 TemplateFamily

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值。 如果无法确定配置类型，则设置为未知。|
|limit|1|指示配置的类型限制是指允许用户注册的设备数。|
|platformRestrictions|2|指示配置属于平台限制类型，指允许用户注册的设备类型。|
|windowsHelloForBusiness|3|指示配置的类型Windows Hello引用设备将使用的身份验证方法。|
|defaultLimit|4|指示配置的类型为默认限制，指默认允许用户注册的设备类型。|
|defaultPlatformRestrictions|5|指示配置属于默认平台限制类型，指默认允许用户注册的设备类型。|
|defaultWindowsHelloForBusiness|6 |指示配置的类型为默认Windows Hello引用默认情况下设备将使用的身份验证方法。|
|defaultWindows10EnrollmentCompletionPageConfiguration|7 |指示配置的类型为默认注册状态页，该页引用默认情况下在 Autopilot 设备的 OOBE 期间显示的启动页。|
|windows10EnrollmentCompletionPageConfiguration|8 |指示配置的类型为“注册状态”页，它引用在 Autopilot 设备的 OOBE 期间显示的启动页。|
|deviceComanagementAuthorityConfiguration|9 |指示配置的类型为 Comanagement Authority，它引用应用于Co-Managed设备的策略。|
|singlePlatformRestriction|10|指示配置属于单一平台限制类型，该限制是指允许用户注册的设备类型。|
|unknownFutureValue|11|未知的未来值|
|enrollmentNotificationsConfiguration|12 |指示配置的类型为注册通知，它引用用户在注册期间收到的通知类型。|





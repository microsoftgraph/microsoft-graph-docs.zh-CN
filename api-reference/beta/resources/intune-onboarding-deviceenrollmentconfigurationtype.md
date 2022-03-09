---
title: deviceEnrollmentConfigurationType 枚举类型
description: 描述 Template 实体的 TemplateFamily
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 85ffeb3b0d8215309b0667be4e0ba874aad66bfa
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63378717"
---
# <a name="deviceenrollmentconfigurationtype-enum-type"></a>deviceEnrollmentConfigurationType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述 Template 实体的 TemplateFamily

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值。 如果无法确定配置类型，则设置为 unknown。|
|limit|1|指示配置的类型限制是指允许用户注册的设备数。|
|platformRestrictions|2|指示配置是平台限制类型，它是指允许用户注册的设备类型。|
|windowsHelloForBusiness|3|指示配置的类型为Windows Hello设备将使用的身份验证方法。|
|defaultLimit|4|指示配置的类型为默认限制，默认限制是指默认情况下允许用户注册的设备类型。|
|defaultPlatformRestrictions|5|指示配置的类型为默认平台限制，该限制指的是默认情况下允许用户注册的设备类型。|
|defaultWindowsHelloForBusiness|6 |指示配置的类型为 default Windows Hello它指的是设备默认将使用的身份验证方法。|
|defaultWindows10EnrollmentCompletionPageConfiguration|7 |指示配置的类型为"默认注册状态"页，该页面指的是默认情况下在 Autopilot 设备中 OOBE 期间显示的启动页面。|
|windows10EnrollmentCompletionPageConfiguration|8 |指示配置的类型为"注册状态"页，该页面是指在 Autopilot 设备中 OOBE 期间显示的启动页面。|
|deviceComanagementAuthorityConfiguration|9 |指示配置的类型为 Comanagement Authority，它引用应用于Co-Managed策略。|
|singlePlatformRestriction|10 |指示配置的类型为单平台限制，该限制是指允许用户注册的设备类型。|
|unknownFutureValue|11|未知未来值|





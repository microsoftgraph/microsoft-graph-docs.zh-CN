---
title: wiFiSecurityType 枚举类型
description: Wi-fi 安全类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 73724041c223d50d0030bf27b780d6b694792a16
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422129"
---
# <a name="wifisecuritytype-enum-type"></a>wiFiSecurityType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Wi-fi 安全类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|打开|0|打开 （无身份验证）。|
|wpaPersonal|1|WPA-个人。|
|wpaEnterprise|2|WPA-企业。 必须使用 IOSEnterpriseWifiConfiguration 类型配置企业选项。|
|wep|3|WEP 加密。|
|wpa2Personal|4|WPA2-个人。|
|wpa2Enterprise|5|WPA2-企业。 必须使用 WindowsWifiEnterpriseEAPConfiguration 类型配置企业选项。|





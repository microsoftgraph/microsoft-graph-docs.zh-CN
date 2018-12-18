---
title: wiFiSecurityType 枚举类型
description: Wi-fi 安全类型。
author: tfitzmac
ms.openlocfilehash: 291bc3660971a90ea113959368542e715a86b570
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329188"
---
# <a name="wifisecuritytype-enum-type"></a>wiFiSecurityType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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






---
title: wiFiSecurityType 枚举类型
description: Wi-fi 安全类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4c770ce8d3e00a8d7997b2b72fcd18eb9007ba83
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787234"
---
# <a name="wifisecuritytype-enum-type"></a>wiFiSecurityType 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Wi-fi 安全类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|open|0|打开（无身份验证）。|
|wpaPersonal|1|WPA-个人版。|
|wpaEnterprise|双面|WPA-企业。 必须使用 IOSEnterpriseWifiConfiguration 类型配置企业选项。|
|wep|第三章|WEP 加密。|
|wpa2Personal|4 |WPA2-个人。|
|wpa2Enterprise|5 |WPA2-企业。 必须使用 WindowsWifiEnterpriseEAPConfiguration 类型配置企业选项。|




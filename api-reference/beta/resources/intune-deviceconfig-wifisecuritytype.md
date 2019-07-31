---
title: wiFiSecurityType 枚举类型
description: Wi-fi 安全类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 33e0e615a62f62a565196ba3a6c9c814695040e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000534"
---
# <a name="wifisecuritytype-enum-type"></a>wiFiSecurityType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Wi-fi 安全类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|open|0|打开 (无身份验证)。|
|wpaPersonal|1|WPA-个人版。|
|wpaEnterprise|双面|WPA-企业。 必须使用 IOSEnterpriseWifiConfiguration 类型配置企业选项。|
|wep|第三章|WEP 加密。|
|wpa2Personal|4|WPA2-个人。|
|wpa2Enterprise|5|WPA2-企业。 必须使用 WindowsWifiEnterpriseEAPConfiguration 类型配置企业选项。|






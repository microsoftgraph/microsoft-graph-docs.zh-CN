---
title: wiFiSecurityType 枚举类型
description: Wi-Fi 安全类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 112612969027be87805b77c5743e1a8d0561c03b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49215335"
---
# <a name="wifisecuritytype-enum-type"></a>wiFiSecurityType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Wi-Fi 安全类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|open|0|打开 (不进行身份验证) 。|
|wpaPersonal|1|WPA-个人版。|
|wpaEnterprise|双面|WPA-企业。 必须使用 IOSEnterpriseWifiConfiguration 类型配置企业选项。|
|wep|第三章|WEP 加密。|
|wpa2Personal|4 |WPA2-个人。|
|wpa2Enterprise|5 |WPA2-企业。 必须使用 WindowsWifiEnterpriseEAPConfiguration 类型配置企业选项。|





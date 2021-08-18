---
title: wiFiSecurityType 枚举类型
description: Wi-Fi安全类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b24b05396a5b436d2c029cfe3991ccbab8cfbce665088d2f67ca62629f7d85c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251412"
---
# <a name="wifisecuritytype-enum-type"></a>wiFiSecurityType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Wi-Fi安全类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|open|0|打开 (身份验证) 。|
|wpaPersonal|1 |WPA-Personal。|
|wpaEnterprise|2 |WPA-Enterprise。 必须使用 IOSEnterpriseWifiConfiguration 类型配置企业选项。|
|wep|3 |WEP 加密。|
|wpa2Personal|4 |WPA2-Personal。|
|wpa2Enterprise|5 |WPA2-Enterprise。 必须使用 WindowsWifiEnterpriseEAPConfiguration 类型配置企业选项。|





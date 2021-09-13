---
title: wiFiSecurityType 枚举类型
description: Wi-Fi安全类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 600173712b5e00f8af9a6e9a94dc4b2167d6130b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057374"
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
|wpaPersonal|1|WPA-Personal。|
|wpaEnterprise|2|WPA-Enterprise。 必须使用 IOSEnterpriseWifiConfiguration 类型配置企业选项。|
|wep|3|WEP 加密。|
|wpa2Personal|4 |WPA2-Personal。|
|wpa2Enterprise|5 |WPA2-Enterprise。 必须使用 WindowsWifiEnterpriseEAPConfiguration 类型配置企业选项。|




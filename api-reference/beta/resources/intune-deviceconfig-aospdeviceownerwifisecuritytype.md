---
title: aospDeviceOwnerWiFiSecurityType 枚举类型
description: Wi-Fi AOSP 设备所有者的安全类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ca3951365d3c8c1c4b17c454526e260184e94dd3
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64631049"
---
# <a name="aospdeviceownerwifisecuritytype-enum-type"></a>aospDeviceOwnerWiFiSecurityType 枚举类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Wi-Fi AOSP 设备所有者的安全类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|open|0|打开 (身份验证) 。|
|wep|1|WEP 加密。|
|wpaPersonal|2|WPA-Personal/WPA2-Personal。|
|wpaEnterprise|4|WPA-Enterprise/WPA2-Enterprise。 必须使用 AOSPDeviceOwnerEnterpriseWifiConfiguration 类型配置企业选项。|





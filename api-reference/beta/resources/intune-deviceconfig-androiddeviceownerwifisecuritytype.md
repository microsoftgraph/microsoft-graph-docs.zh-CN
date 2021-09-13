---
title: androidDeviceOwnerWiFiSecurityType 枚举类型
description: Wi-Fi Android 设备所有者的安全类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 02895e68b36d000731cc606f3abb1dbd942146c9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081421"
---
# <a name="androiddeviceownerwifisecuritytype-enum-type"></a>androidDeviceOwnerWiFiSecurityType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Wi-Fi Android 设备所有者的安全类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|open|0|打开 (身份验证) 。|
|wep|1|WEP 加密。|
|wpaPersonal|2|WPA-Personal/WPA2-Personal。|
|wpaEnterprise|4 |WPA-Enterprise/WPA2-Enterprise。 必须使用 AndroidDeviceOwnerEnterpriseWifiConfiguration 类型配置企业选项。|




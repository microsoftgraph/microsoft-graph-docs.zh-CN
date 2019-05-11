---
title: androidDeviceOwnerWiFiSecurityType 枚举类型
description: Android 设备所有者的 Wi-fi 安全类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b015aa8c2e56df0a919b580d09f1a1d7e8bbe0c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33948987"
---
# <a name="androiddeviceownerwifisecuritytype-enum-type"></a>androidDeviceOwnerWiFiSecurityType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 设备所有者的 Wi-fi 安全类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|open|0|打开 (无身份验证)。|
|wep|1|WEP 加密。|
|wpaPersonal|双面|WPA-个人/WPA2-个人。|
|wpaEnterprise|4|WPA-企业/WPA2-企业。 必须使用 AndroidDeviceOwnerEnterpriseWifiConfiguration 类型配置企业选项。|





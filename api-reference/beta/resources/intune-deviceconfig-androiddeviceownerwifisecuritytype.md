---
title: androidDeviceOwnerWiFiSecurityType 枚举类型
description: 适用于 Android 设备所有者的 Wi-Fi 安全类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6763f1fd20be16c297e75979ca934511a005e379
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734047"
---
# <a name="androiddeviceownerwifisecuritytype-enum-type"></a>androidDeviceOwnerWiFiSecurityType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

适用于 Android 设备所有者的 Wi-Fi 安全类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|open|0|打开 (不进行身份验证) 。|
|wep|1|WEP 加密。|
|wpaPersonal|双面|WPA-个人/WPA2-个人。|
|wpaEnterprise|4 |WPA-企业/WPA2-企业。 必须使用 AndroidDeviceOwnerEnterpriseWifiConfiguration 类型配置企业选项。|






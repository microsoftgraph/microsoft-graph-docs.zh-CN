---
title: androidDeviceOwnerWiFiSecurityType 枚举类型
description: 适用于 Android 设备所有者的 Wi-Fi 安全类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 742c21c0358cab27050d75e94065bb788ceec6fa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294835"
---
# <a name="androiddeviceownerwifisecuritytype-enum-type"></a>androidDeviceOwnerWiFiSecurityType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

适用于 Android 设备所有者的 Wi-Fi 安全类型。

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|open|0|打开 (不进行身份验证) 。|
|wep|1|WEP 加密。|
|wpaPersonal|双面|WPA-个人/WPA2-个人。|
|wpaEnterprise|4 |WPA-企业/WPA2-企业。 必须使用 AndroidDeviceOwnerEnterpriseWifiConfiguration 类型配置企业选项。|





---
title: deviceManagementConfigurationTechnologies 枚举类型
description: 介绍此设置可以使用哪种技术进行部署
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d9d65d7e2bb44f6886be35362d2de07386ec84b
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670539"
---
# <a name="devicemanagementconfigurationtechnologies-enum-type"></a>deviceManagementConfigurationTechnologies 枚举类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

介绍此设置可以使用哪种技术进行部署

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无法通过任何通道部署设置|
|Mdm|1|可以通过 MDM 通道部署设置|
|windows10XManagement|2|可以通过 Windows10XManagement 通道部署设置|
|configManager|4|可以通过 ConfigManager 通道部署设置|
|appleRemoteManagement|64|可以通过 AppleRemoteManagement 通道部署设置|
|microsoftSense|128|可以通过 SENSE 代理通道部署设置|
|exchangeOnline|256|可以通过Exchange Online代理通道部署设置|
|linuxMdm|1024|可以通过 Linux Mdm 通道部署设置|
|招生|4096|可以通过设备注册部署设置。|
|unknownFutureValue|1073741824|对于客户端无法处理新枚举值的情况，Sentinel 成员。|





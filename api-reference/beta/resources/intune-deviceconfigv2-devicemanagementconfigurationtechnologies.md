---
title: deviceManagementConfigurationTechnologies 枚举类型
description: 描述可以使用哪种技术部署此设置
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d7766d88b7670a4cd0a96a3e4a52a462478a9a41
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148184"
---
# <a name="devicemanagementconfigurationtechnologies-enum-type"></a>deviceManagementConfigurationTechnologies 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述可以使用哪种技术部署此设置

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无法通过任何通道部署设置|
|mdm|1|可通过 MDM 通道部署设置|
|windows10XManagement|2|可通过 Windows10XManagement 通道部署设置|
|configManager|4 |可通过 ConfigManager 通道部署设置|
|microsoftSense|128|可以通过 SENSE 代理通道部署设置|
|exchangeOnline|256|可以通过代理通道部署Exchange Online设置|




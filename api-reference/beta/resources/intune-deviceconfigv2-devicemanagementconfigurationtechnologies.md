---
title: deviceManagementConfigurationTechnologies 枚举类型
description: 描述可以使用哪种技术部署此设置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9c935c1f69e843940a9e4aa29199dbfd9b5a02aa3528f7612c72055ab3f2efbc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54185794"
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
|mdm|1 |可通过 MDM 通道部署设置|
|windows10XManagement|2 |可通过 Windows10XManagement 通道部署设置|
|configManager|4 |可通过 ConfigManager 通道部署设置|
|microsoftSense|128|可以通过 SENSE 代理通道部署设置|





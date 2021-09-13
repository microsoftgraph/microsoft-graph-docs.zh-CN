---
title: operatingSystemUpgradeEligibility 枚举类型
description: 从任意位置工作 Windows 设备升级资格状态
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 498f08baf98ae1de1a650ae8b3e071761a357672
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091319"
---
# <a name="operatingsystemupgradeeligibility-enum-type"></a>operatingSystemUpgradeEligibility 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

从任意位置工作 Windows 设备升级资格状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|upgraded|0|设备已升级到最新版本的 Windows|
|unknown|1|没有足够的数据可用于计算设备对 Windows 升级的资格|
|notCapable|2|设备无法进行 Windows 升级|
|capable|3|设备支持 Windows 升级|




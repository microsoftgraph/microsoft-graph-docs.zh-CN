---
title: operatingSystemUpgradeEligibility 枚举类型
description: 从任意位置工作 Windows 设备升级资格状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3a6871d0168324a01e7d9a8ef39b8164e453ff2e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805708"
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




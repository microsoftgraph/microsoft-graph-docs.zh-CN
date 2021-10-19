---
title: androidDeviceOwnerEnrollmentMode 枚举类型
description: 注册配置文件的注册模式。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e369682fda379ce8d4b4905839be42ca4ff523c5
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60487210"
---
# <a name="androiddeviceownerenrollmentmode-enum-type"></a>androidDeviceOwnerEnrollmentMode 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

注册配置文件的注册模式。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|corporateOwnedDedicatedDevice|0|尚未记录|
|corporateOwnedFullyManaged|1|尚未记录|
|corporateOwnedWorkProfile|2|尚未记录|
|corporateOwnedAOSPUserlessDevice|3|企业拥有、无用户 Android 开放Project (AOSP) 设备，无需 Google 移动服务。|
|corporateOwnedAOSPUserAssociatedDevice|4 |企业拥有的、与用户关联的 Android 开放源代码Project (AOSP) 设备，无需 Google 移动服务。|




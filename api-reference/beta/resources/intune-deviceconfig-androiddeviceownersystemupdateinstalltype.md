---
title: androidDeviceOwnerSystemUpdateInstallType 枚举类型
description: Android 设备所有者的系统更新类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 13b983ca2c017646108d6076ebcc3a92652165c0de28691c6390875443f6df04
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54190652"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a>androidDeviceOwnerSystemUpdateInstallType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 设备所有者的系统更新类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认行为，通常提示用户接受系统更新。|
|postpone|1 |将更新的自动安装推迟至 30 天。|
|窗口|2 |在日常维护时段内自动安装。|
|自动|3 |尽快自动安装更新。|





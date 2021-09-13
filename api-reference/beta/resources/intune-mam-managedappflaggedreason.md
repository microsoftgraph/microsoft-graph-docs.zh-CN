---
title: managedAppFlaggedReason 枚举类型
description: 用户被标记的原因
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b139ce9aaf192473d835a001fd71d9dfca710d40
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075086"
---
# <a name="managedappflaggedreason-enum-type"></a>managedAppFlaggedReason 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户被标记的原因

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|没有问题。|
|rootDevice|1|应用注册正在根/解锁的设备上运行。|
|androidBootloaderUnlocked|2|应用注册正在解锁启动加载程序的 Android 设备上运行。|
|androidFactoryRomModified|3|应用注册正在已修改工厂 ROM 的 Android 设备上运行。|




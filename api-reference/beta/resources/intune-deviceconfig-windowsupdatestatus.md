---
title: windowsUpdateStatus 枚举类型
description: Windows配置设备状态更新
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 73404f8d01ab6ea047cb94ecc3b21939e4fb3a6c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803803"
---
# <a name="windowsupdatestatus-enum-type"></a>windowsUpdateStatus 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows配置设备状态更新

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|upToDate|0|没有挂起的更新、没有挂起的重启更新和失败的更新。|
|pendingInstallation|1|存在挂起安装的更新，其中包括未批准的更新。 没有挂起的重启更新，没有失败的更新。|
|pendingReboot|2|有些更新需要重新启动。 没有失败的更新。|
|failed|3|在设备上安装更新失败。|




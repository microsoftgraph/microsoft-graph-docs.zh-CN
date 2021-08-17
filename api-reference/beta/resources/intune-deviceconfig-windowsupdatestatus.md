---
title: windowsUpdateStatus 枚举类型
description: Windows配置设备状态更新
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7da061fafd5ed59c215031b2e2626c8d0d42a50661089e9646455ae6d96c4668
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54213156"
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
|pendingInstallation|1 |存在挂起安装的更新，其中包括未批准的更新。 没有挂起的重启更新，没有失败的更新。|
|pendingReboot|2 |有些更新需要重新启动。 没有失败的更新。|
|failed|3 |在设备上安装更新失败。|





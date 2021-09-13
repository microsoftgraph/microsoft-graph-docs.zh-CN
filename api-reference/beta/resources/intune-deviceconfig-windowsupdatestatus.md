---
title: windowsUpdateStatus 枚举类型
description: Windows配置设备状态更新
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b07580a4057ba79e932a442d38bac323936df751
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075387"
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




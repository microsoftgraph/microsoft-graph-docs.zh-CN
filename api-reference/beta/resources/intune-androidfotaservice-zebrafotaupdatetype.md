---
title: zebraFotaUpdateType 枚举类型
description: 表示 Zebra FOTA 部署的各种更新类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5bd17423e3a158a2010ae0afac18b56e406e1651
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213173"
---
# <a name="zebrafotaupdatetype-enum-type"></a>zebraFotaUpdateType 枚举类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 Zebra FOTA 部署的各种更新类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|自 定义|0|自定义更新，用户选择要更新到的特定 BSP、OS 版本和修补程序编号。|
|最新|1|最新发布的更新将成为目标 OS。 最新版本可能会将设备更新到新的 Android 版本。|
|自动|2|设备始终查找存储库中提供的最新包，并在有新包可用时尝试更新。 这会一直持续到管理员取消自动更新为止。|
|unknownFutureValue|99|未知的未来枚举值。|





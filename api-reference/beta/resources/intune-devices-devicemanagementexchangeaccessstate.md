---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 309f3ead8ae67d3dda4c8c6f6d6a27a701f96d21
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388351"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a>deviceManagementExchangeAccessState 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备交换访问状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|没有从 Exchange 中发现的访问状态|
|unknown|1|Exchange 的设备访问状态未知|
|支持|双面|设备有权访问 Exchange|
|堵塞|第三章|设备在 Exchange 中被阻止|
|隔离|4 |Exchange 中的设备被隔离|




---
title: actionState 枚举类型
description: 设备上操作的状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7f805b39ac3954981c368ac79e566d3dc4fc218c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760214"
---
# <a name="actionstate-enum-type"></a>actionState 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备上操作的状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|操作状态无效|
|pending|1|操作挂起|
|canceled|2|操作已取消。|
|active|3|操作处于活动状态。|
|done|4 |操作已完成，没有错误。|
|failed|5 |操作失败|
|notSupported|6 |不支持操作。|





---
title: actionState 枚举类型
description: 设备上的操作状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3b559fd45e4ffe36c5c111e50738eea4c195161a
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734205"
---
# <a name="actionstate-enum-type"></a>actionState 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备上的操作状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无效的操作状态|
|等待|1|操作正在挂起|
|取消|2|操作已取消。|
|积极|3|操作处于活动状态。|
|done|4|操作已完成，没有错误。|
|失败|5|操作失败|
|notSupported|6 |不支持操作。|






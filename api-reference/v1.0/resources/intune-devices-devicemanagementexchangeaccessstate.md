---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ef97c75379a446c0dc503636e8870dfe14f52ee2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533289"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a>deviceManagementExchangeAccessState 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备交换访问状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|没有从 Exchange 中发现的访问状态|
|unknown|1 |Exchange 的设备访问状态未知|
|支持|2 |设备有权访问 Exchange|
|堵塞|3 |设备在 Exchange 中被阻止|
|隔离|4 |Exchange 中的设备被隔离|





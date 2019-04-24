---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fedbd157c4668397256971c57a4cb5fa355f78c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584661"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a>deviceManagementExchangeAccessState 枚举类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备交换访问状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|没有从 Exchange 中发现的访问状态|
|unknown|1|Exchange 的设备访问状态未知|
|支持|2 |设备有权访问 Exchange|
|堵塞|3 |设备在 Exchange 中被阻止|
|隔离|4 |Exchange 中的设备被隔离|




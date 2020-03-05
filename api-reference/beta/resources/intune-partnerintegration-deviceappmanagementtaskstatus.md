---
title: deviceAppManagementTaskStatus 枚举类型
description: 设备应用程序管理任务状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6819f5ad7ab0cc9f931392a55371fe555b9bc1a6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524025"
---
# <a name="deviceappmanagementtaskstatus-enum-type"></a>deviceAppManagementTaskStatus 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备应用程序管理任务状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|状态未定义。|
|决|1 |任务已准备好进行审阅。|
|工作|2 |任务已被接受，正在进行处理。|
|后|3 |工作已完成。|
|拒绝|4 |任务已被拒绝。|




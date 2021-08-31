---
title: deviceAppManagementTaskStatus 枚举类型
description: 设备应用管理任务状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9cd78446eeac6096ac212401e55c2b5767cc3f68
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58784182"
---
# <a name="deviceappmanagementtaskstatus-enum-type"></a>deviceAppManagementTaskStatus 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备应用管理任务状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未定义状态。|
|pending|1|任务已准备好进行审阅。|
|active|2|任务已被接受且正在处理中。|
|已完成|3|工作已完成。|
|rejected|4 |任务被拒绝。|




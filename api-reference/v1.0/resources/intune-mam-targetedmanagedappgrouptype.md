---
title: targetedManagedAppGroupType 枚举类型
description: 指示要面向的应用集合，这些应用可以是几个预定义的应用列表之一或手动选择的应用列表之一
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e7c6dd39ff11f961f93d844a1b85f38f634ee343
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730586"
---
# <a name="targetedmanagedappgrouptype-enum-type"></a>targetedManagedAppGroupType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示要面向的应用集合，这些应用可以是几个预定义的应用列表之一或手动选择的应用列表之一

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|selectedPublicApps|0|面向管理员手动选择的应用集合。|
|allCoreMicrosoftApps|1|将 Microsoft 应用的核心集 (Office、Edge 等) 为目标。|
|allMicrosoftApps|2|将 Microsoft 作为发布者的所有应用作为目标。|
|allApps|4|面向具有可用分配的所有应用。|






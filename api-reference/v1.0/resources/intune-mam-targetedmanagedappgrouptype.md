---
title: targetedManagedAppGroupType 枚举类型
description: 指示要面向的应用集合，这些应用可以是多个预定义的应用列表之一或手动选择的应用列表
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 21813297d3774c32838828d6eacaca3dc684b7b5
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60454458"
---
# <a name="targetedmanagedappgrouptype-enum-type"></a>targetedManagedAppGroupType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示要面向的应用集合，这些应用可以是多个预定义的应用列表之一或手动选择的应用列表

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|selectedPublicApps|0|面向管理员手动选择的应用集合。|
|allCoreMicrosoftApps|1|面向 Microsoft 应用的核心集 (Office、Edge 等) 。|
|allMicrosoftApps|2|将 Microsoft 作为发布者面向所有应用。|
|allApps|4 |面向具有可用分配的所有应用。|




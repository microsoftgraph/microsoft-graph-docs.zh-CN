---
title: groupPolicyMigrationReadiness 枚举类型
description: 指示组策略对象文件是否已被覆盖并准备好进行 Intune 迁移。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 15e7d0a626934f8f6d17aebf6eff9aff8c537dbd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031226"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a>groupPolicyMigrationReadiness 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示组策略对象文件是否已被覆盖并准备好进行 Intune 迁移。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|1 |无 Intune 覆盖范围|
|环|2 |部分 Intune 覆盖范围|
|complete|第三章|完成 Intune 覆盖范围|
|error|4 |分析覆盖率时出错|
|notApplicable|5 |GPO 中没有组策略设置|







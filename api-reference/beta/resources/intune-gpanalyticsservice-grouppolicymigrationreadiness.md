---
title: groupPolicyMigrationReadiness 枚举类型
description: 指示是否覆盖组策略对象文件并准备进行 Intune 迁移。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1b65c8f739e4c93d8881e12b8b715e4bfc7aa7ef
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057304"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a>groupPolicyMigrationReadiness 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示是否覆盖组策略对象文件并准备进行 Intune 迁移。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|1|无 Intune 覆盖范围|
|partial|2|部分 Intune 覆盖范围|
|complete|3|完整的 Intune 覆盖范围|
|error|4 |分析覆盖范围时出错|
|notApplicable|5 |GPO 中无组策略设置|




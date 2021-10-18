---
title: appListType 枚举类型
description: 合规性应用列表的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a5410919bb33a4a77d4d774108157519fad9ae4d
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60455919"
---
# <a name="applisttype-enum-type"></a>appListType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

合规性应用列表的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|默认值，无意图。|
|appsInListCompliant|1|该列表表示将被视为合规的应用 (只有列表中的应用符合) 。|
|appsNotInListCompliant|2|该列表表示被视为不合规的应用 (所有应用都合规，列表上的应用除外) 。|




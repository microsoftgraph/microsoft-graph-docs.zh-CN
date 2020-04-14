---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 61999950fbf9a54a2d93576fe77d950e30b8b561
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469950"
---
# <a name="applisttype-enum-type"></a>appListType 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

合规性应用程序列表的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|默认值，无意向。|
|appsInListCompliant|1|此列表表示将被视为合规性的应用程序（仅符合列表中的应用程序）。|
|appsNotInListCompliant|双面|此列表表示将被视为不合规的应用程序（所有应用程序都符合列表中的应用程序）。|




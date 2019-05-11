---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 98d7f8a71f12dd70eb062a1e6eff5c5c3054fd40
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947552"
---
# <a name="applisttype-enum-type"></a>appListType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

合规性应用程序列表的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|默认值, 无意向。|
|appsInListCompliant|1|此列表表示将被视为合规性的应用程序 (仅符合列表中的应用程序)。|
|appsNotInListCompliant|双面|此列表表示将被视为不合规的应用程序 (所有应用程序都符合列表中的应用程序)。|





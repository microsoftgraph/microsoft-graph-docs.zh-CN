---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5df56b14d3c5416a04245ffbccd0b3b887266bde
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987787"
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






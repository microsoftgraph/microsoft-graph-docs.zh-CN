---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7cd3e1f8cffa747ca23e00ba0d9264cb1089dee2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260815"
---
# <a name="applisttype-enum-type"></a>appListType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

合规性应用程序列表的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|默认值，无意向。|
|appsInListCompliant|1|此列表代表只有列表中的应用程序符合标准的应用程序，才会被视为合规 (性的) 。|
|appsNotInListCompliant|双面|此列表表示将被视为不合规的应用程序 (所有应用程序不符合列表) 中的应用程序。|





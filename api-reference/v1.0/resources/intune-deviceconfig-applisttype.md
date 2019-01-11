---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 76c13c26812fd8ab7c8e1224b55e616502b514ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839268"
---
# <a name="applisttype-enum-type"></a>appListType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

合规性应用程序列表的可能值。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|无|0|默认值，没有用途。|
|appsInListCompliant|1|在列表代表将被视为符合 （仅在列表上的应用程序都符合） 的应用程序。|
|appsNotInListCompliant|2|在列表代表将被视为不符合标准的应用程序 （所有应用程序是除列表上的应用程序兼容）。|




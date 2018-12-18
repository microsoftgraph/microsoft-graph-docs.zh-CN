---
title: Members
description: 介绍 teamsApp 的当前安装状态。
author: nkramer
ms.openlocfilehash: a73c68298c4cdf65deee68fb3bd707d50bc2475a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316791"
---
#<a name="teamsappinstalledstate-enum-type"></a>teamsAppInstalledState 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

介绍[teamsApp](teamsapp.md)的当前安装状态。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|notInstalled|0|应用程序并不安装到团队。|
|安装|1|通常安装应用程序。|
|installedAndHidden|2|应用程序是安装，但从视图中隐藏。|
|installedAndPermanent|3|应用程序永久安装，并且不会删除。|

---
title: macOSSoftwareUpdateState 枚举类型
description: MacOS 软件更新状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 05d2d951d8eacb93d952e20f01af6e42b30eecc1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731076"
---
# <a name="macossoftwareupdatestate-enum-type"></a>macOSSoftwareUpdateState 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS 软件更新状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|success|0|成功安装软件更新|
|下载|1000|正在下载软件更新|
|完毕|1001|已下载软件更新|
|安装|1002|正在安装软件更新|
|待机|1003|对此软件更新不执行任何操作|
|可用|1004|软件更新在设备上可用|
|scheduled|1005|已在设备上安排软件更新|
|downloadFailed|2000|软件更新下载失败|
|downloadInsufficientSpace|2001|空间不足，无法下载更新|
|downloadInsufficientPower|2002|没有足够的功率来下载更新|
|downloadInsufficientNetwork|2003|网络容量不足，无法下载更新|
|installInsufficientSpace|2004|空间不足，无法安装更新|
|installInsufficientPower|2005|没有足够的电源来安装更新|
|installFailed|2006|安装因未指定原因而失败|
|commandFailed|2007|由于未指定的原因，计划更新命令失败|






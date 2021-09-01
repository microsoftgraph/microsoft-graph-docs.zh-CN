---
title: macOSSoftwareUpdateState 枚举类型
description: MacOS 软件更新状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 45720943bd4050b0a72ad0a6cdb13356adb7e8f5
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806955"
---
# <a name="macossoftwareupdatestate-enum-type"></a>macOSSoftwareUpdateState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS 软件更新状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|success|0|已成功安装软件更新|
|下载|1000|正在下载软件更新|
|已下载|1001|已下载软件更新|
|安装|1002|正在安装软件更新|
|idle|1003|对此软件更新未采取任何操作|
|可用|1004|软件更新在设备上可用|
|scheduled|1005|已在设备上计划软件更新|
|downloadFailed|2000|软件更新下载失败|
|downloadInsufficientSpace|2001|没有足够的空间来下载更新|
|downloadInsufficientPower|2002|没有足够的电源来下载更新|
|downloadInsufficientNetwork|2003|网络容量不足，无法下载更新|
|installInsufficientSpace|2004|没有足够的空间来安装更新|
|installInsufficientPower|2005|没有足够的电源来安装更新|
|installFailed|2006|由于未指定的原因，安装失败|
|commandFailed|2007|计划更新命令因未指定的原因失败|




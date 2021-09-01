---
title: windowsSModeConfiguration 枚举类型
description: 配置 S 模式解锁的可能选项
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e0a650246725b478d980ca0fe46063838142032e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58816541"
---
# <a name="windowssmodeconfiguration-enum-type"></a>windowsSModeConfiguration 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

配置 S 模式解锁的可能选项

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|noRestriction|0|此选项将删除解锁 S 模式的所有限制 - 默认|
|block|1|此选项将阻止用户从 S 模式解锁设备|
|unlock|2|此选项将在 S 模式下解锁设备|




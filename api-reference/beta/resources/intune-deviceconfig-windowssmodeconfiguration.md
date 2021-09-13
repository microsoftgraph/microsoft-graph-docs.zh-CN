---
title: windowsSModeConfiguration 枚举类型
description: 配置 S 模式解锁的可能选项
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c3c06f2888b7d7c9e7a7af2736a93e233b4c1475
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59105872"
---
# <a name="windowssmodeconfiguration-enum-type"></a>windowsSModeConfiguration 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

配置 S 模式解锁的可能选项

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noRestriction|0|此选项将删除解锁 S 模式的所有限制 - 默认|
|block|1|此选项将阻止用户从 S 模式解锁设备|
|unlock|2|此选项将在 S 模式下解锁设备|




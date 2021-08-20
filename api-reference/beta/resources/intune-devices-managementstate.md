---
title: managementState 枚举类型
description: 设备在设备中的Microsoft Intune。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1475ac4dc29462b31df57ae54daf4ecb658487133ad5b0fe2cc5884e8effdc5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249872"
---
# <a name="managementstate-enum-type"></a>managementState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备在设备中的Microsoft Intune。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|托管|0|设备正在管理中|
|retirePending|1 |停用命令在设备上发生，并且正在从管理中注销|
|retireFailed|2 |停用命令在设备上失败|
|wipePending|3 |擦除命令在设备上发生，并且正在取消注册管理|
|wipeFailed|4 |擦除命令在设备上失败|
|不正常|5 |设备不正常。|
|deletePending|6 |在设备上执行删除命令 |
|retireIssued|7 |为设备发布了停用命令|
|wipeIssued|8 |为设备发出擦除命令|
|wipeCanceled|9 |此设备的擦除命令已取消|
|retireCanceled|10 |此设备的停用命令已取消|
|已发现|11 |已发现设备，但设备未完全注册。|





---
title: windowsUpdateType 枚举类型
description: 哪些分支设备将接收其更新
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9d6ab79b8d0320a3830948ef1e2973f158338310849618c47b45cbcc9c20253f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244887"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

哪些分支设备将接收其更新

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|允许用户设置。|
|all|1 |半年频道 (定向) 。 设备从半年频道和目标用户获取 (功能) 。|
|businessReadyOnly|2 |半年频道。 设备从半年频道获取功能更新。|
|windowsInsiderBuildFast|3 |Windows预览体验成员内部版本 - 快速|
|windowsInsiderBuildSlow|4 |Windows预览体验成员内部版本 - 慢|
|windowsInsiderBuildRelease|5 |预览Windows内部版本|





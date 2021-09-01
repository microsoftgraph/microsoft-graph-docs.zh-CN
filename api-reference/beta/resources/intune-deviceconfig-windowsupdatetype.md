---
title: windowsUpdateType 枚举类型
description: 哪些分支设备将接收其更新
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d052a6f746fb37e936c2eb37126efd31cd74a7d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796851"
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
|all|1|半年频道 (定向) 。 设备从半年频道和目标用户获取 (功能) 。|
|businessReadyOnly|2|半年频道。 设备从半年频道获取功能更新。|
|windowsInsiderBuildFast|3|Windows预览体验成员内部版本 - 快速|
|windowsInsiderBuildSlow|4 |Windows预览体验成员内部版本 - 慢|
|windowsInsiderBuildRelease|5 |预览Windows内部版本|




---
title: defenderMonitorFileActivity 枚举类型
description: 监视文件活动的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bb3d16f9ff70de4e7457b31a5a48307e9fa48fdb
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58759685"
---
# <a name="defendermonitorfileactivity-enum-type"></a>defenderMonitorFileActivity 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

监视文件活动的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|用户定义，默认值，无意图。|
|disable|1|禁用监视文件活动。|
|monitorAllFiles|2|监视所有文件。|
|monitorIncomingFilesOnly|3| 仅监视传入文件。|
|monitorOutgoingFilesOnly|4 |仅监视传出文件。|




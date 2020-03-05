---
title: defenderRealtimeScanDirection 枚举类型
description: 监视文件活动的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0256c756be59b1b3661360d4c952a385fd5c6348
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526869"
---
# <a name="defenderrealtimescandirection-enum-type"></a>defenderRealtimeScanDirection 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

监视文件活动的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|monitorAllFiles|0|0（默认值）–监视所有文件（双向）|
|monitorIncomingFilesOnly|1 |仅监视传入的文件。|
|monitorOutgoingFilesOnly|2 |仅监视传出文件。|




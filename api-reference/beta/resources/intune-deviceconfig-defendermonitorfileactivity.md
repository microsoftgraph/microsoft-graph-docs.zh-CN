---
title: defenderMonitorFileActivity 枚举类型
description: 监视文件活动的可能值。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c0ec26e3883e6ab30bdd41fe96b2e6f2bbd90d74
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040496"
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




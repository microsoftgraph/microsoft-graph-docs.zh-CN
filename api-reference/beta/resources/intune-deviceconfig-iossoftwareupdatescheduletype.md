---
title: iosSoftwareUpdateScheduleType 枚举类型
description: 更新 iOS 软件更新的计划类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4629ddd0aba60cfd71956eea07f05ce4119eee7f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111157"
---
# <a name="iossoftwareupdatescheduletype-enum-type"></a>iosSoftwareUpdateScheduleType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 iOS 软件更新的计划类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|updateOutsideOfActiveHours|0|在使用时段之外更新。|
|alwaysUpdate|1|始终更新。|
|updateDuringTimeWindows|2|在时间窗口期间更新。|
|updateOutsideOfTimeWindows|3|在时间窗口之外更新。|




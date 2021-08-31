---
title: remediationState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: dad0c6030d4a0f06ac17da9f2060b099d71d4ea4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788932"
---
# <a name="remediationstate-enum-type"></a>remediationState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示设备管理脚本的执行状态的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|结果未知。|
|已跳过|1|已跳过修正脚本执行|
|success|2|修复脚本成功执行并修正设备状态|
|remediationFailed|3|修正脚本已成功执行，但未能修正设备状态|
|scriptError|4 |修正脚本执行遇到的错误或时间过长|




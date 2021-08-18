---
title: edgeKioskModeRestrictionType 枚举类型
description: 指定如何Microsoft Edge展台模式限制用户设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 34c87657e6add9011a1533383a3d549c4e609be6f921435fe7c622a1bc207a9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145409"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a>edgeKioskModeRestrictionType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定如何Microsoft Edge展台模式限制用户设置。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置 (无限制) 。|
|digitalSignage|1 |单应用模式下的交互式/数字标志。|
|normalMode|2 |正常模式 (完整版本的Microsoft Edge) 。|
|publicBrowsingSingleApp|3 |单应用模式下的公共浏览。|
|publicBrowsingMultiApp|4 |在多 (模式下) InPrivate 中的公共浏览功能。|





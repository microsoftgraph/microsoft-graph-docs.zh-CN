---
title: safeSearchFilterType 枚举类型
description: 指定筛选成人内容 (需要的安全) 级别
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: adf5460c702b5779591152d5241cf66f22af0e6f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091620"
---
# <a name="safesearchfiltertype-enum-type"></a>safeSearchFilterType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定筛选成人内容 (需要的安全) 级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|用户定义，默认值，无意图。|
|strict|1|对成人内容进行严格、最高的筛选。|
|中等|2|对成人内容进行适量 (不会筛选出有效的) 。|




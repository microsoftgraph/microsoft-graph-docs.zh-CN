---
title: appListType 枚举类型
description: 合规性应用列表的可能值。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: eab8857585226f84fcba2014cb72827ef5e0fd6f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59069360"
---
# <a name="applisttype-enum-type"></a>appListType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

合规性应用列表的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|默认值，无意图。|
|appsInListCompliant|1|该列表表示将被视为合规的应用 (只有列表上的应用符合) 。|
|appsNotInListCompliant|2|该列表表示将视为不合规的应用 (除了列表上的应用之外的所有应用都) 。|




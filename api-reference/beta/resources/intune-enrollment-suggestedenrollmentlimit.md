---
title: suggestedEnrollmentLimit 资源类型
description: suggestedEnrollmentLimit 资源表示在给定注册类型时建议的注册限制。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fca3ed6ad1d885fd01bc1aa313253a46b9acb4d7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054336"
---
# <a name="suggestedenrollmentlimit-resource-type"></a>suggestedEnrollmentLimit 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

suggestedEnrollmentLimit 资源表示在给定注册类型时建议的注册限制。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|suggestedDailyLimit|Int32|一天内建议的注册限制|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.suggestedEnrollmentLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.suggestedEnrollmentLimit",
  "suggestedDailyLimit": 1024
}
```




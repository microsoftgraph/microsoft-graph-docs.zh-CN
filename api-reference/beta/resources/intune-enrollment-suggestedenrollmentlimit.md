---
title: suggestedEnrollmentLimit 资源类型
description: suggestedEnrollmentLimit 资源表示在给定注册类型时建议的注册限制。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7595aa2ab614a7c9abb0ac9c76c4b05fda1288eea7b11c24b2b1932a1265a321
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54197938"
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





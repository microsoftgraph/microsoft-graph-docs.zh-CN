---
title: educationOnPremisesInfo 资源类型
description: 用于将本地 Active Directory 用户帐户关联到其 Azure AD 用户对象的其他信息。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c461c63309588fc01fef94fb53a3b9c6e0f2722858f1baaa93a663804e344b7c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182530"
---
# <a name="educationonpremisesinfo-resource-type"></a>educationOnPremisesInfo 资源类型

命名空间：microsoft.graph

用于将本地 Active Directory 用户帐户关联到其 Azure AD 用户对象的其他信息。

## <a name="properties"></a>属性

| 属性    | 类型   | 说明                                                |
| :---------- | :----- | :--------------------------------------------------------- |
| immutableId | String | Active Directory 中用户对象的唯一标识符。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationOnPremisesInfo"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationOnPremisesInfo",
  "immutableId": "String"
}
```

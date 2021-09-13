---
title: educationOnPremisesInfo 资源类型
description: 用于将本地 Active Directory 用户帐户关联到其 Azure AD 用户对象的其他信息。
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ace4f32edf7a708debea828bfc510aec630a7100
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078887"
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

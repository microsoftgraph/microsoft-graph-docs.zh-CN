---
title: accessPackageResourceAttributeQuestion 资源类型
description: 用于定义提供给最终用户的问题的资源，以获取要传递给最终系统或请求审批者的属性值。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5ced0c1e769000f3624681d92dade18cf8dddcc9
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468280"
---
# <a name="accesspackageresourceattributequestion-resource-type"></a>accessPackageResourceAttributeQuestion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于 [定义提供给最终用户](accesspackagequestion.md) 的问题的资源，以获取要传递给最终系统或请求审批者的属性值。

此类型继承自 [accessPackageResourceAttributeSource](../resources/accesspackageresourceattributesource.md)，并用于 [accessPackageResourceAttribute 的 attributeSource 属性](accesspackageresourceattribute.md)。

唯一的属性是 **question**，可以是 [accessPackageTextInputQuestion](accesspackagetextinputquestion.md) 或 [accessPackageMultipleChoiceQuestion](accesspackagemultiplechoicequestion.md) 对象类型。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|question|accessPackageQuestion|为了获取属性的值而询问的问题|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttributeQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttributeQuestion",
  "question": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  }
}
```

---
title: identityCustomUserFlowAttribute 资源类型
description: 表示 Azure Active Directory 租户中可用于自助服务注册用户流的自定义用户流属性。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3a07ea64be3cf5a215c43271982b7fdfce3f6662
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882658"
---
# <a name="identitycustomuserflowattribute-resource-type"></a>identityCustomUserFlowAttribute 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure Active Directory 租户中可用于自助服务注册用户流的自定义用户流属性。 这些属性无法修改且为只读。

继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户流属性的标识符。 这是一个自动创建的只读属性。 继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)|
|displayName|String|用户流属性的显示名称。 继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)|
|说明|String|注册时显示给用户的用户流量属性的描述。 继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)|
|userFlowAttributeType|identityUserFlowAttributeType|用户流属性的类型。 这是一个自动设置的只读属性。 此属性的值将为 `custom` 。 继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。|
|DataType|identityUserFlowAttributeDataType|用户流属性的数据类型。 在创建自定义用户流属性后，不能对此进行修改。 数据类型 **支持** 为： `string` 、 `boolean` 、 `int64` 、 `stringCollection` 、 `dateTime`。 继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityCustomUserFlowAttribute",
  "baseType": "microsoft.graph.identityUserFlowAttribute",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityCustomUserFlowAttribute",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "userFlowAttributeType": "String",
  "dataType": "String"
}
```

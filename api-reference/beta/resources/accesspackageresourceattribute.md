---
title: accessPackageResourceAttribute 资源类型
description: 公开访问包请求者的属性的资源，以提供可用于为访问包做出审批决策的自定义信息。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 27fdb3e5cf90b3a4a7d691b2c44c1d8b36a7d9ab
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468291"
---
# <a name="accesspackageresourceattribute-resource-type"></a>accessPackageResourceAttribute 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

访问包资源属性是用户必须能够访问应用程序所需的属性的定义。 此结构包含在目录的 [accessPackageResource](../resources/accesspackageresource.md) 中，用于其角色包含在该目录的访问包中的应用程序。 当用户请求访问包时，他们必须提供 属性的值，如果请求得到批准，则该值将写入用户的目录对象。 然后，应用程序可以 [读取用户的属性](../api/user-get.md)。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|attributeDestination|[accessPackageResourceAttributeDestination](../resources/accesspackageresourceattributedestination.md)|有关如何设置属性的信息（当前为 [accessPackageUserDirectoryAttributeStore](accesspackageuserdirectoryattributestore.md) 对象类型）。|
|attributeName|String|最终系统中属性的名称。 如果目标为 `accessPackageUserDirectoryAttributeStore`，则用户属性（如 **jobTitle** ）或用户的目录架构扩展对象类型，例如 `extension_2b676109c7c74ae2b41549205f1947ed_personalTitle`。 |
|attributeSource|[accessPackageResourceAttributeSource](../resources/accesspackageresourceattributesource.md)|有关在 **满足 accessPackageAssignmentRequest** 时如何填充属性值的信息，当前 [accessPackageResourceAttributeQuestion](accesspackageresourceattributequestion.md) 对象类型。|
|id|String|访问包资源上属性的唯一标识符。 只读。 |
|isEditable|字符串| 指定请求者是否可以编辑现有属性值。|
|isPersistedOnAssignmentRemoval|布尔| 指定属性在工作分配结束后是否仍保留在最终系统中。|


### <a name="accesspackageresourceattribute-resource-type-and-extension-properties"></a>accessPackageResourceAttribute 资源类型和扩展属性

访问 **包资源属性的 attributeDestination**、 **attributeName** 和 **attributeSource** 属性与 [目录扩展属性相关](extensionproperty.md)。

如果 **attributeDestination** 是 [accessPackageUserDirectoryAttributeStore](accesspackageuserdirectoryattributestore.md) 对象类型，则 **attributeName** 指示的属性必须是用户对象的可 [写](user.md) 属性。 这些可写属性是已注册为目标 User 对象的 [扩展属性](extensionproperty.md) 的 **String** 类型。

例如，假设应用程序需要两个用户属性，即用户职务和个人职务。 这些属性的值可以同步到Azure AD Active Directory **jobTitle** 和 **personalTitle** 属性的值。 由于 **personalTitle** 不是用户对象的默认属性之一，因此 [](user.md)将需要创建目录架构扩展以 [](../api/application-post-extensionproperty.md)将 **personalTitle** 属性添加到用户对象类型。 为应用程序创建资源请求时，可以包含两个访问包资源属性，一个属性用于用户属性 **jobTitle**`extension_2b676109c7c74ae2b41549205f1947ed_personalTitle`，另一个属性具有为个人标题创建的目录架构扩展属性的名称，例如 。

如果属性的 **attributeSource** 是 [accessPackageResourceAttributeQuestion](accesspackageresourceattributequestion.md)，则请求者提供的值将存储为用户对象上提供的值，并且可用于应用程序和其他 Microsoft Graph 客户端。
## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttribute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttribute",
  "attributeDestination": {
    "@odata.type": "microsoft.graph.accessPackageResourceAttributeDestination"
  },
  "attributeName": "String",
  "attributeSource": {
    "@odata.type": "microsoft.graph.accessPackageResourceAttributeSource"
  },
  "id": "String (identifier)",
  "isEditable": "Boolean",
  "isPersistedOnAssignmentRemoval": "Boolean"
}
```

---
title: 标识资源类型
description: 表示一个标识，用于设置对添加到 Microsoft Graph 的外部内容的权限。
author: sacampbe-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: fd1b5ce0cb828e4c409062a8fcb05f51c82a943f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123382"
---
# <a name="identity-resource-type"></a>标识资源类型

命名空间：microsoft.graph.externalConnectors

表示[一个](externalconnectors-identity.md)标识，用于设置对添加到 Microsoft Graph 的外部内容的权限。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[创建标识](../api/externalconnectors-externalgroup-post-members.md)|[identity](externalconnectors-identity.md)|为 [externalGroup](../resources/externalconnectors-identity.md) 中的新成员创建 [标识资源](../resources/externalconnectors-externalgroup.md)。|
|[删除标识](../api/externalconnectors-identity-delete.md)|无|删除 [标识](../resources/externalconnectors-identity.md) 资源以从 [externalGroup 中删除相应的成员](../resources/externalconnectors-externalgroup.md)。|

## <a name="properties"></a>属性

| 属性       | 类型                    | 说明                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| id             | String                  | 标识的唯一 ID。 对于使用 Azure AD 的用户或组Azure Active Directory (，它将是 objectId 属性) 对于外部组，则为 **externalGroup** 的 **id** 属性。                                    |
| type           | microsoft.graph.externalConnectors.identityType | 标识的类型。 可能的值包括： `user` 或 `group` Azure AD 标识和 `externalgroup` 外部系统中组的值。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.identity",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "type": "String"
}
```

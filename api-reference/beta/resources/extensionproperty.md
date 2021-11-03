---
title: extensionProperty 资源类型
description: 表示目录扩展
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 5768603fd68c883e7b2ee722f11366fe6dfabfe9
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696222"
---
# <a name="extensionproperty-resource-type"></a>extensionProperty 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个目录扩展，可用于向目录对象添加自定义属性，而无需外部数据存储。 例如，如果组织的业务线 (LOB) 应用程序需要目录中每个用户的 Skype ID，则 Microsoft Graph 可用于在目录的 User 对象上注册名为 skypeId 的新属性，然后将值写入特定用户的新属性。

可以将扩展添加到[用户](user.md)、组、[组织、](organization.md)[设备](device.md)[、应用程序](application.md)资源。 [](group.md) 所有类型和所有应用程序中只能将 100个扩展值写入任何单个Azure AD资源。 

> [!IMPORTANT]
> Azure AD介绍的架构扩展在 Microsoft Graph中仅出于向后兼容性原因提供。
> 它允许你使用 Microsoft Graph管理通过已弃用Azure AD Graph (或[) 添加](/azure/active-directory/hybrid/whatis-azure-ad-connect)Azure AD 连接。
> 对于新的自定义扩展，建议使用 Microsoft Graph架构扩展[向资源添加自定义数据](/graph/extensibility-overview)。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出扩展](../api/application-list-extensionproperty.md) | [extensionProperty](extensionProperty.md) 集合 | 列出应用程序对象上的扩展属性。 |
| [创建扩展](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | 在应用程序对象上创建扩展属性。 |
| [删除扩展](../api/application-delete-extensionproperty.md) | 无 | 从应用程序对象删除扩展属性。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|appDisplayName|String| 定义此扩展属性的应用程序对象的显示名称。 只读。 |
|DataType|String| 指定数据类型属性可以保留的值的值的值。 支持以下值。 不可为 null。 <ul><li>`Binary` - 最多 256 个字节</li><li>`Boolean`</li><li>`DateTime` - 必须以 ISO 8601 格式指定。 存储为 UTC 格式。</li><li>`Integer` - 32 位值。</li><li>`LargeInteger` - 64 位值。</li><li>`String` - 最多 256 个字符</li></ul>|
|isSyncedFromOnPremises|布尔值| 指示是否使用此扩展属性从 onpremises 目录Azure AD 连接。 只读。 |
|name|String| 扩展属性的名称。 不可为 null。 |
|targetObjects|String collection| 支持以下值。 不可为空。 <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionProperty",
  "keyProperty": "id"
}-->

```json
{
  "appDisplayName": "String",
  "dataType": "String",
  "isSyncedFromOnPremises": true,
  "name": "String",
  "targetObjects": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

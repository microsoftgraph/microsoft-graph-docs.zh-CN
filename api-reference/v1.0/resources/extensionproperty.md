---
title: extensionProperty 资源类型
description: 表示目录扩展
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 03fe00fc3da41e3885311e92bb5979c91d8b4db3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336786"
---
# <a name="extensionproperty-resource-type"></a>extensionProperty 资源类型

命名空间：microsoft.graph

表示一个目录扩展，可用于向目录对象添加自定义属性，而无需外部数据存储。 例如，如果组织的业务线 (LOB) 应用程序需要目录中每个用户的 Skype ID，则 Microsoft Graph 可用于在目录的 User 对象上注册名为 skypeId 的新属性，然后为特定用户的新属性写入值。

可以将扩展添加到[用户](user.md)、[组](group.md)、[组织、](organization.md)[设备](device.md)[、应用程序](application.md)资源。 所有类型和所有应用程序中只能将 100  个扩展值写入任何单个Azure AD资源。

> [!IMPORTANT]
> Azure AD介绍的架构扩展在 Microsoft Graph中仅出于向后兼容性原因提供。
> 它允许你使用 Microsoft Graph管理通过已弃用Azure AD Graph (或) 添加的扩展[Azure AD 连接](/azure/active-directory/hybrid/whatis-azure-ad-connect)。
> 对于新的自定义扩展，建议使用 Microsoft Graph架构扩展[向资源添加自定义数据](/graph/extensibility-overview)。

继承自 [directoryObject](directoryobject.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 extensionProperties](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | 在应用程序对象上创建扩展属性。 |
| [列出 extensionProperties](../api/application-list-extensionproperty.md) | [extensionProperty](extensionProperty.md) 集合 | 列出应用程序对象上的扩展属性。 |
| [获取 extensionProperty](../api/extensionproperty-get.md) | [extensionProperty](extensionProperty.md) 集合 | 列出应用程序对象上的扩展属性。 |
| [删除 extensionProperty](../api/extensionproperty-delete.md) | 无 | 从应用程序对象删除扩展属性。 |

> [!TIP]
> 1. 若要将扩展属性的值设置为 **targetObjects** 中指定的资源实例，请使用资源的 Update 操作。 例如，更新 [用户](../api/user-update.md) API 以设置用户的值。
> 2. 若要从 **targetObjects** 中指定的资源实例中删除扩展属性及其值，将扩展属性的值设置为 `null`。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|appDisplayName|String| 定义此扩展属性的应用程序对象的显示名称。 只读。 |
|DataType|String| 指定数据类型属性可以保留的值的值的值。 支持以下值。 不可为 null。 <ul><li>`Binary` - 最多 256 个字节</li><li>`Boolean`</li><li>`DateTime` - 必须以 ISO 8601 格式指定。 存储为 UTC 格式。</li><li>`Integer` - 32 位值。</li><li>`LargeInteger` - 64 位值。</li><li>`String` - 最多 256 个字符</li></ul>|
|deletedDateTime|DateTimeOffset|删除此对象的日期和时间。 始终 `null` 在对象尚未删除时。 继承自 [directoryObject](directoryobject.md)。|
|isSyncedFromOnPremises|Boolean| 指示此扩展属性是否使用 Azure AD 连接。 只读。 |
|name|String| 扩展属性的名称。 不可为 null。 |
|targetObjects|String 集合| 支持以下值。 不可为空。 <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.extensionProperty",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extensionProperty",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "name": "String",
  "dataType": "String",
  "isSyncedFromOnPremises": "Boolean",
  "targetObjects": [
    "String"
  ]
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

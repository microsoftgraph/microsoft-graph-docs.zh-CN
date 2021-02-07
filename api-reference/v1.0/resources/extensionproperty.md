---
title: extensionProperty 资源类型
description: 表示目录扩展
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a9e16eaed46cb23609d437b09f25eb59a3ce9616
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131276"
---
# <a name="extensionproperty-resource-type"></a>extensionProperty 资源类型

命名空间：microsoft.graph

表示可用于向目录对象添加自定义属性而无需外部数据存储的目录扩展。 例如，如果组织有一个业务线 (LOB) 应用程序，该应用程序需要目录中每个用户的 Skype ID，则 Microsoft Graph 可用于在目录的用户对象上注册名为 skypeId 的新属性，然后为特定用户的新属性写入值。

可以将扩展添加到[用户、组](user.md)、[组织、](organization.md)[设备](device.md)[、应用程序](application.md)资源。 [](group.md)

> [!IMPORTANT]
> 此处所述的 Azure AD 架构扩展仅在出于向后兼容性原因才可在 Microsoft Graph 中提供。
> 它允许你使用 Microsoft Graph 继续管理通过 Azure AD Graph 或 [Azure AD Connect 添加的扩展属性](/azure/active-directory/hybrid/whatis-azure-ad-connect)。
> 对于新的自定义扩展，建议使用 Microsoft Graph 架构扩展将 [自定义数据添加到资源](/graph/extensibility-overview)。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建扩展](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | 在应用程序对象上创建扩展属性。 |
| [列出扩展](../api/application-list-extensionproperty.md) | [extensionProperty](extensionProperty.md) 集合 | 列出应用程序对象上的扩展属性。 |
| [删除扩展](../api/application-delete-extensionproperty.md) | 无 | 从应用程序对象删除扩展属性。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|appDisplayName|String| 定义此扩展属性的应用程序对象的显示名称。 只读。 |
|DataType|String| 指定数据类型属性可以保留的值的默认值。 支持以下值。 不可为 null。 <ul><li>`Binary` - 最多 256 字节</li><li>`Boolean`</li><li>`DateTime` - 必须以 ISO 8601 格式指定。 存储为 UTC 格式。</li><li>`Integer` - 32 位值。</li><li>`LargeInteger` - 64 位值。</li><li>`String` - 最多 256 个字符</li></ul>|
|isSyncedFromOnPremises|布尔| 指示此扩展属性是否从使用 Azure AD Connect 的 onpremises 目录中获取。 只读。 |
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
  "baseType": "",
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

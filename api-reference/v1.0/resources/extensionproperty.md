---
title: extensionProperty 资源类型
description: 表示目录扩展
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 81bda27c0bee96fbac30e4f586e5ffb4a78bac09
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939500"
---
# <a name="extensionproperty-resource-type"></a>extensionProperty 资源类型

表示可用于将自定义属性添加到目录对象而不需要外部数据存储区的目录扩展。 例如，如果组织具有需要目录中每个用户的 Skype ID 的业务线（LOB）应用程序，则可以使用 Microsoft Graph 在目录的 User 对象上注册一个名为 skypeId 的新属性，然后向新属性中写入一个值特定用户的。

可以将扩展添加到[用户](user.md)、[组](group.md)、[组织](organization.md)、[设备](device.md)、[应用程序](application.md)资源。

> [!IMPORTANT]
> 此处介绍的 Azure AD 架构扩展在 Microsoft Graph 中可用，仅用于向后兼容的原因。
> 它允许您使用 Microsoft Graph 继续管理通过 Azure AD Graph 或[AZURE Ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect)添加的扩展属性。
> 对于新的自定义扩展，我们建议使用 Microsoft Graph 架构扩展[将自定义数据添加到资源](/graph/extensibility-overview)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建扩展](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | 在 application 对象上创建扩展属性。 |
| [列表扩展](../api/application-list-extensionproperty.md) | [extensionProperty](extensionProperty.md)集合 | 列出应用程序对象上的扩展属性。 |
| [删除扩展](../api/application-delete-extensionproperty.md) | 无 | 从 application 对象中删除扩展属性。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|appDisplayName|String| 在其上定义此扩展属性的 application 对象的显示名称。 只读。 |
|DataType|String| 指定 extension 属性可以包含的值的数据类型。 支持以下值。 不可为空。 <ul><li>`Binary`-最多为256字节</li><li>`Boolean`</li><li>`DateTime`-必须以 ISO 8601 格式指定。 存储为 UTC 格式。</li><li>`Integer`-32-位值。</li><li>`LargeInteger`-64-位值。</li><li>`String`-最多为-256 个字符</li></ul>|
|isSyncedFromOnPremises|Boolean| 指示是否使用 Azure AD Connect 从 onpremises 目录中 sycned 此扩展属性。 只读。 |
|name|字符串| 扩展属性的名称。 不可为空。 |
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

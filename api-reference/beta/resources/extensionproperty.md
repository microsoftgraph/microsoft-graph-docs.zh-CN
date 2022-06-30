---
title: extensionProperty 资源类型
description: 表示目录扩展
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8de2c18fb4f6ea5b6d2a91f453b915ee7f9b93ea
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556379"
---
# <a name="extensionproperty-resource-type"></a>extensionProperty 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个目录扩展，可用于将自定义属性添加到目录对象，而无需外部数据存储。 例如，如果组织有业务线 (LOB) 需要目录中每个用户的 Skype ID 的应用程序，则可以使用 Microsoft Graph 在目录的 User 对象上注册名为 skypeId 的新属性，然后为特定用户将值写入新属性。

可将目录扩展添加到以下目录对象：
+ [user](user.md)
+ [group](group.md)
+ [组织](organization.md)
+ [设备](device.md)
+ [应用程序](application.md) 资源

在 *所有* 类型和 *所有* 应用程序中，只能将 100 个扩展值写入任何单个 Azure AD 资源实例。

使用此资源和关联的方法来管理目录扩展定义。 若要管理扩展资源实例上的目录扩展数据，请使用用于管理资源实例的同一 REST 请求。

有关 Microsoft Graph 扩展性的详细信息，请 [参阅使用扩展向资源添加自定义属性](/graph/extensibility-overview)。

继承自 [directoryObject](directoryobject.md)。

> [!NOTE]
> 通过 Azure AD Graph 创建的扩展 (已弃用) 和使用 Azure AD Connect Sync 从本地 Active Directory同步的自定义数据表示为 Microsoft Graph 中的目录扩展。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 extensionProperties](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | 在应用程序对象上创建扩展属性。 |
| [列出 extensionProperties](../api/application-list-extensionproperty.md) | [extensionProperty](extensionProperty.md) 集合 | 列出应用程序对象上的扩展属性。 |
| [获取 extensionProperty](../api/extensionproperty-get.md) | [extensionProperty](extensionProperty.md) 集合 | 列出应用程序对象上的扩展属性。 |
| [删除 extensionProperty](../api/extensionproperty-delete.md) | 无 | 从应用程序对象删除扩展属性。 只能删除未从本地 Active Directory 同步的属性。 |

> [!TIP]
> 1. 若要将扩展属性的值设置为 **targetObjects** 中指定的资源的实例，请使用资源的更新操作。 例如，要为用户设置值的 [更新用户](../api/user-update.md) API。
> 2. 若要从 **targetObjects** 中指定的资源实例中删除扩展属性及其值，请将扩展属性的值设置为 `null`。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|appDisplayName|String| 在其中定义此扩展属性的应用程序对象的显示名称。 只读。 |
|DataType|String| 指定扩展属性可以保存的值的数据类型。 支持以下值。 不可为 null。 <ul><li>`Binary` - 最大 256 字节数</li><li>`Boolean`</li><li>`DateTime` - 必须以 ISO 8601 格式指定。 存储为 UTC 格式。</li><li>`Integer` - 32 位值。</li><li>`LargeInteger` - 64 位值。</li><li>`String` - 最大 256 个字符</li></ul>|
|deletedDateTime|DateTimeOffset|删除此对象的日期和时间。 在对象尚未删除时始终为 `null`。 继承自 [directoryObject](directoryobject.md)。|
|isSyncedFromOnPremises|Boolean| 指示此扩展属性是否已使用 Azure AD Connect 从本地 Active Directory 同步。 只读。 |
|name|String| 扩展属性的名称。 不可为 null。 |
|targetObjects|字符串集合| 支持以下值。 不可为空。 <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

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

## <a name="see-also"></a>另请参阅

+ [使用扩展将自定义属性添加到资源](/graph/extensibility-overview)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

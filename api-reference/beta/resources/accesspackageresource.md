---
title: accessPackageResource 资源类型
description: 访问包资源是一个对与目录关联的资源的引用，该目录的角色可在一个或多个访问包中使用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e34b850b19836eeb19cc63232c7af822512bfee4
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934820"
---
# <a name="accesspackageresource-resource-type"></a>accessPackageResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利](entitlementmanagement-root.md)管理中，访问包资源是一个对与访问包目录（可在一个或多个访问包中使用的角色）关联的资源的引用。  若要请求将资源与访问包目录关联，或者从目录中删除资源，请创建[accessPackageResourceRequest。](accesspackageresourcerequest.md)

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageCatalog 资源](../api/accesspackagecatalog-list-accesspackageresources.md) | [accessPackageResource](accesspackageresource.md) 集合 | 检索目录中的 accessPackageResource 对象列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|addedBy|String|只读。|
|addedOn|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|说明|String|资源的说明。|
|displayName|String|资源的显示名称，如应用程序名称、组名称或网站名称。|
|id|String| 只读。|
|isPendingOnboarding|Boolean|如果资源尚未可用于工作分配，则其为 True。|
|originId|String|源系统中资源的唯一标识符。 对于 Azure AD 组，这是该组的标识符。 |
|originSystem|String|源系统中资源的类型，例如 `SharePointOnline` ， `AadApplication` 或 `AadGroup` 。|
|resourceType|String|资源的类型，例如它是 Azure `Application` AD 连接的应用程序或 `SharePoint Online Site` SharePoint Online 网站。|
|url|String|资源的唯一资源定位器，例如用于将用户登录应用程序的 URL。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageResourceRoles|[accessPackageResourceRole](accesspackageresourcerole.md) 集合| 只读。 可为 Null。|
|accessPackageResourceScopes|[accessPackageResourceScope](accesspackageresourcescope.md) 集合| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResource",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "addedBy": "String",
  "addedOn": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isPendingOnboarding": true,
  "originId": "String",
  "originSystem": "String",
  "resourceType": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



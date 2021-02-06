---
title: accessPackageResource 资源类型
description: 访问包资源是一个对与目录关联的资源的引用，该目录的角色可在一个或多个访问包中使用。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 31499fda1d2d12f1e9868da6cf9e09fde38298cd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137464"
---
# <a name="accesspackageresource-resource-type"></a>accessPackageResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包资源是一个对与访问包目录关联的资源的引用。 访问包资源的角色可在一个或多个访问包中使用。  若要请求将资源与访问包目录关联，或者从目录中删除资源，请创建[accessPackageResourceRequest。](accesspackageresourcerequest.md)

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageCatalog 资源](../api/accesspackagecatalog-list-accesspackageresources.md) | [accessPackageResource](accesspackageresource.md) 集合 | 检索目录中的 accessPackageResource 对象列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageResourceEnvironment|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|包含资源的环境信息。 这可以使用批注或 `@odata.bind` 环境的 *originId 进行设置*。|
|addedBy|字符串|只读。|
|addedOn|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|说明|字符串|资源的说明。|
|displayName|字符串|资源的显示名称，如应用程序名称、组名称或网站名称。|
|id|字符串| 只读。|
|isPendingOnboarding|Boolean|如果资源尚未可用于工作分配，则其为 True。|
|originId|字符串|源系统中资源的唯一标识符。 对于 Azure AD 组，这是组的标识符。 |
|originSystem|字符串|源系统中资源的类型，例如 `SharePointOnline` ， `AadApplication` 或 `AadGroup` 。|
|resourceType|字符串|资源的类型，例如 `Application` 它是已连接 Azure AD 的应用程序还是 `SharePoint Online Site` SharePoint Online 网站。|
|url|String|资源的唯一资源定位器，例如用于将用户登录应用程序的 URL。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageResourceEnvironment|[accessPackageResourceEnvironment](accesspackageresourceenvironment.md)| 可为 NULL。|
|accessPackageResourceRoles|[accessPackageResourceRole](accesspackageresourcerole.md) 集合| 只读。 可为 NULL。|
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

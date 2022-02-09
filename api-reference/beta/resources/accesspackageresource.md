---
title: accessPackageResource 资源类型
description: 访问包资源是一个对与目录关联的资源的引用，该目录的角色可在一个或多个访问包中使用。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 867e4e400175cd912b90b79aadfd64591bedfb7b
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468340"
---
# <a name="accesspackageresource-resource-type"></a>accessPackageResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD中](entitlementmanagement-overview.md)，访问包资源是一个对与访问包目录关联的资源的引用。 访问包资源的角色可在一个或多个访问包中使用。  若要请求将资源与访问包目录关联，或者从目录中删除资源，请创建 [accessPackageResourceRequest](accesspackageresourcerequest.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageCatalog 资源](../api/accesspackagecatalog-list-accesspackageresources.md) | [accessPackageResource](accesspackageresource.md) 集合 | 检索目录中的 accessPackageResource 对象列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageResourceEnvironment|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|包含资源的环境信息。 这可以使用批注或 `@odata.bind` 环境的 *originId 进行设置*。|
|attributes|[accessPackageResourceAttribute](../resources/accesspackageresourceattribute.md) 集合| 包含有关从请求程序收集并发送到资源应用程序的属性的信息。 |
|addedBy|String|只读。|
|addedOn|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|description|String|资源的说明。|
|displayName|String|资源的显示名称，如应用程序名称、组名称或网站名称。|
|id|String| 只读。|
|isPendingOnboarding|布尔|如此 如果资源尚不可用于工作分配。|
|originId|String|源系统中资源的唯一标识符。 对于组Azure AD，这是组的标识符。 |
|originSystem|字符串|源系统中资源的类型 `SharePointOnline`，如 或 `AadApplication` `AadGroup`。|
|resourceType|String|资源的类型`Application`，例如，它是已Azure AD应用程序`SharePoint Online Site`，还是 SharePoint Online 网站。|
|url|String|资源的唯一资源定位器，例如用于将用户登录应用程序的 URL。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageResourceEnvironment|[accessPackageResourceEnvironment](accesspackageresourceenvironment.md)| 可为 NULL。 支持 `$expand`。|
|accessPackageResourceRoles|[accessPackageResourceRole](accesspackageresourcerole.md) 集合| 只读。 可为 NULL。 支持 `$expand`。|
|accessPackageResourceScopes|[accessPackageResourceScope](accesspackageresourcescope.md) 集合| 只读。 可为 NULL。 支持 `$expand`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResource",
  "keyProperty": "id"
}-->

```json
{
  "addedBy": "String",
  "addedOn": "String (timestamp)",
  "attributes": [
    {
      "@odata.type": "microsoft.graph.accessPackageResourceAttribute"
    }
   ],
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

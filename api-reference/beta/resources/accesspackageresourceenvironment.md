---
title: accessPackageResourceEnvironment 资源类型
description: 访问包资源环境是资源所在的地理位置环境的引用。
author: hanki-microsoft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0a1d9362371b9a479d12ba6613e49854283bd610
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651194"
---
# <a name="accesspackageresourceenvironment-resource-type"></a>accessPackageResourceEnvironment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD中](entitlementmanagement-overview.md)，访问包资源环境是资源所在的地理位置环境的引用。 此环境将自动作为权利管理的一Azure AD提供。 此 API 仅适用于多地理位置SharePoint在线网站。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessPackageResourceEnvironments](../api/entitlementmanagement-list-accesspackageresourceenvironment.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 集合|检索 [accessPackageResourceEnvironment 对象](../resources/accesspackageresourceenvironment.md) 的列表。|
|[获取 accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|读取 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|connectionInfo|[connectionInfo](../resources/connectioninfo.md)|用于连接到资源的环境的连接信息。 |
|createdBy|String|创建显示名称的用户的组。|
|createdDateTime|DateTimeOffset|创建此对象的日期和时间。 <br>DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|说明|String|此对象的说明。|
|displayName|String|此显示名称对象的对象。|
|id|String|系统分配的对象的唯一标识符。|
|isDefaultEnvironment|Boolean|确定这是否是默认环境。 它设置为所有 `true` 静态源系统，如Azure AD组和 Azure AD Applications。|
|modifiedBy|String|最后显示名称修改此对象的实体的子项。|
|modifiedDateTime|DateTimeOffset|上次修改此对象的日期和时间。 <br>DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
|originId|String|源系统中此环境的唯一标识符。|
|originSystem|String|源系统中资源的类型，即 `SharePointOnline` 。 需要 `$filter` `eq` () 。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|accessPackageResources|[accessPackageResource](../resources/accesspackageresource.md) 集合|只读。 必需。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceEnvironment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceEnvironment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "originSystem": "String",
  "originId": "String",
  "isDefaultEnvironment": "Boolean",
  "connectionInfo": {
    "@odata.type": "microsoft.graph.connectionInfo"
  },
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```

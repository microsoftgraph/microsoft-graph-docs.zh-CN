---
title: accessPackageResourceEnvironment 资源类型
description: 访问包资源环境是资源所在的地理位置环境的引用。
author: hanki-microsoft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b21c0f1ae8fd70ac2df76dfa50bc886bca04de19
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760853"
---
# <a name="accesspackageresourceenvironment-resource-type"></a>accessPackageResourceEnvironment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包资源环境是资源所在的地理位置环境的引用。 此环境自动作为 Azure AD 权利管理的一部分提供。 此 API 仅适用于多地理位置 SharePoint Online 网站。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessPackageResourceEnvironments](../api/accesspackageresourceenvironment-list.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 集合|检索 [accessPackageResourceEnvironment 对象](../resources/accesspackageresourceenvironment.md) 的列表。|
|[获取 accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|读取 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|connectionInfo|[connectionInfo](../resources/connectioninfo.md)|用于连接到资源的环境的连接信息。 |
|createdBy|String|创建显示名称的用户的组。|
|createdDateTime|DateTimeOffset|创建此对象的日期和时间。 <br>DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|说明|String|此 *accessPackageResourceEnvironment 对象的* 说明。|
|displayName|String|此显示名称对象的对象。|
|id|String|系统分配的对象的唯一标识符。|
|isDefaultEnvironment|布尔|确定这是否是默认环境。 它设置为 `true` 所有静态源系统，如 Azure AD 组和 Azure AD 应用程序。|
|modifiedBy|String|最后显示名称修改此对象的实体的子项。|
|modifiedDateTime|DateTimeOffset|上次修改此对象的日期和时间。 <br>DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
|originId|String|源系统中此环境的唯一标识符。|
|originSystem|String|源系统中资源的类型，例如 `SharePointOnline` 。 支持 `$filter`。|

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

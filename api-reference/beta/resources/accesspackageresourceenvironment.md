---
title: accessPackageResourceEnvironment 资源类型
description: 访问包资源环境是资源所在的地理位置环境的引用。
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 814e77cb8122773bc425180c7e78a2794c9e0784
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137697"
---
# <a name="accesspackageresourceenvironment-resource-type"></a>accessPackageResourceEnvironment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包资源环境是资源所在的地理位置环境的引用。 此环境自动作为 Azure AD Entilement 管理的一部分提供。 此 API 仅适用于多地理位置 SharePoint Online 网站。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessPackageResourceEnvironments](../api/accesspackageresourceenvironment-list.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 集合|检索 [accessPackageResourceEnvironment 对象](../resources/accesspackageresourceenvironment.md) 的列表。|
|[获取 accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|读取 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|connectionInfo|[connectionInfo](../resources/connectioninfo.md)|用于连接到资源的环境的连接信息。 |
|createdBy|String|创建显示名称的用户的用户名。|
|createdDateTime|DateTimeOffset|创建此对象的日期和时间。 <br>DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `'2014-01-01T00:00:00Z'` 。|
|说明|字符串|此 *accessPackageResourceEnvironment 对象的* 说明。|
|displayName|字符串|此显示名称对象的属性。|
|id|字符串|系统分配的对象的唯一标识符。|
|isDefaultEnvironment|Boolean|确定这是否是默认环境。 它设置为所有 `true` 静态源系统，如 Azure AD 组和 Azure AD 应用程序。|
|modifiedBy|字符串|最后显示名称修改此对象的实体的项。|
|modifiedDateTime|DateTimeOffset|上次修改此对象的日期和时间。 <br>DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `'2014-01-01T00:00:00Z'` 。 |
|originId|字符串|源系统中此环境的唯一标识符。|
|originSystem|字符串|源系统中资源的类型，例如 `SharePointOnline` 。 支持 `$filter`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|accessPackageResources|[accessPackageResource](../resources/accesspackageresource.md) 集合|只读。 必填。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceEnvironment",
  "baseType": "",
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

---
title: userSource 资源类型
description: 保管人邮箱和 OneDrive for business 网站的容器。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 2ce5448947bded580cc4896ba549d7cc6fab95f9
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597512"
---
# <a name="usersource-resource-type"></a>userSource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[保管人](custodian.md)邮箱和 OneDrive for business 网站的容器。

## <a name="methods"></a>方法

|方法|返回类型|Description|
|:---|:---|:---|
|[列出 userSources](../api/custodian-list-usersources.md)|[userSource](../resources/usersource.md) 集合|获取 **userSource** 对象及其属性的列表。|
|[创建 userSource](../api/custodian-post-usersources.md)|[userSource](../resources/usersource.md)|创建新的 **userSource** 对象。|
|[获取 userSource](../api/usersource-get.md)|[userSource](../resources/usersource.md)|读取 **userSource** 对象的属性和关系。|
|[删除 userSource](../api/usersource-delete.md)|无|删除 **userSource** 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **userSource** 的用户。|
|createdDateTime|DateTimeOffset|美国 **userSource** erSource 的创建日期和时间|
|displayName|String|与邮箱和网站关联的显示名称。|
|email|String|用户邮箱的电子邮件地址。|
|id|String|**UserSource** 的 ID。 这不是实际组的 ID|
|includedSources|sourceType|指定要包含在此组中的源。 可取值为：`mailbox`、`site`。|

### <a name="sourcetype-values"></a>sourceType 值

与用户相关的源的类型。 默认情况下包括邮箱和网站。

|成员|说明|
|:----|-----------|
|邮箱|代表一个邮箱。|
|网站|表示 OneDrive for business 网站。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSource",
  "baseType": "microsoft.graph.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "email": "String",
  "includedSources": "String"
}
```

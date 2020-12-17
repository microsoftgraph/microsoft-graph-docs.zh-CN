---
title: userSource 资源类型
description: 保管人邮箱和 OneDrive for Business 网站的容器。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 10184e053a0c62aaba6599f7d6f9bb6a33de8828
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706036"
---
# <a name="usersource-resource-type"></a>userSource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

保管人邮箱 [和](custodian.md) OneDrive for Business 网站的容器。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userSources](../api/custodian-list-usersources.md)|[userSource](../resources/usersource.md) 集合|获取 **userSource 对象** 及其属性的列表。|
|[创建 userSource](../api/custodian-post-usersources.md)|[userSource](../resources/usersource.md)|创建新的 **userSource** 对象。|
|[获取 userSource](../api/usersource-get.md)|[userSource](../resources/usersource.md)|读取 **userSource** 对象的属性和关系。|
|[删除 userSource](../api/usersource-delete.md)|无|删除 **userSource** 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **userSource 的用户**。|
|createdDateTime|DateTimeOffset|创建 **userSource 的** 日期和时间|
|displayName|字符串|与显示名称和网站关联的邮箱。|
|email|字符串|用户邮箱的电子邮件地址。|
|id|字符串|userSource 的ID。 这不是实际组的 ID|
|includedSources|sourceType|指定此组中包含的源。 可取值为：`mailbox`、`site`。|

### <a name="sourcetype-values"></a>sourceType 值

与用户相关的源类型。 默认情况下包括邮箱和网站。

|成员|说明|
|:----|-----------|
|邮箱|表示邮箱。|
|网站|代表 OneDrive for Business 网站。|

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

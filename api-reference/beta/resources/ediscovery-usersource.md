---
title: userSource 资源类型
description: 保管人邮箱和 OneDrive for Business 网站的容器。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f0d98ac894d3d60bed2bb249ef9daec707f6f7ba
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446650"
---
# <a name="usersource-resource-type"></a>userSource 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

保管人邮箱 [和](ediscovery-custodian.md) OneDrive for Business 网站的容器。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userSources](../api/ediscovery-custodian-list-usersources.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 集合|获取 **userSource 对象** 及其属性的列表。|
|[创建 userSource](../api/ediscovery-custodian-post-usersources.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|创建新的 **userSource** 对象。|
|[获取 userSource](../api/ediscovery-usersource-get.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|读取 **userSource** 对象的属性和关系。|
|[删除 userSource](../api/ediscovery-usersource-delete.md)|无|删除 **userSource** 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **userSource 的用户**。|
|createdDateTime|DateTimeOffset|创建 **userSource** 的日期和时间|
|displayName|String|与显示名称和网站关联的邮箱。|
|email|String|用户邮箱的电子邮件地址。|
|id|String|userSource 的ID。 这不是实际组的 ID|
|includedSources|microsoft.graph.ediscovery.sourceType|指定此组中包含的源。 可取值为：`mailbox`、`site`。|

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
  "@odata.type": "microsoft.graph.ediscovery.userSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.userSource",
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

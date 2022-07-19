---
title: userSource 资源类型
description: 用户邮箱和OneDrive for Business网站的容器。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b36d9cc2947c263510c8b08d05f210a556985690
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838176"
---
# <a name="usersource-resource-type"></a>userSource 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用户邮箱和OneDrive for Business网站的容器。

继承自 [dataSource](../resources/security-datasource.md)。

## <a name="methods"></a>方法
无。 
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **userSource 的用户**。|
|createdDateTime|DateTimeOffset|用户 **源** 的创建日期和时间。|
|displayName|String|与邮箱和网站关联的显示名称。|
|email|String|Email用户邮箱的地址。|
|id|String|**userSource** 的 ID。 这不是实际组的 ID。|
|includedSources|microsoft.graph.security.sourceType|指定此组中包含的源。 可取值为：`mailbox`、`site`。|
|siteWebUrl|String|用户OneDrive for Business站点的 URL。 只读。|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|**userSource** 的保留状态。 可能的值包括 `notApplied`、`applied`、`applying`、`removing`、`partial`。|


### <a name="usersourceholdstatus-values"></a>userSourceHoldStatus 值

|名称|说明|
|:----|-----------|
|notApplied|userSource 未保留 (其中的所有源都未保留) 。|
|应用|userSource 处于保留状态 (所有源都处于保留状态) 。|
|应用|userSource 正在应用保留状态 (已触发的 applyHold 操作) 。|
|删除|userSource 正在删除 () 触发的 removeHold 操作的保留状态。|
|部分|userSource 处于混合状态，其中某些源处于保留状态，有些源未处于保留或错误状态。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.userSource",
  "baseType": "microsoft.graph.security.dataSource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.userSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "email": "String",
  "includedSources": "String",
  "siteWebUrl": "String"
}
```
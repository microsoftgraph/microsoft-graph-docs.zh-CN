---
title: userSource 资源类型
description: 用户邮箱和 OneDrive for Business 网站的容器。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 45bd3444baa6b3e0aa7c13f6678fd9c2312915b5
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945146"
---
# <a name="usersource-resource-type"></a>userSource 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用户邮箱和 OneDrive for Business 网站的容器。

继承自 [dataSource](../resources/security-datasource.md)。

## <a name="methods"></a>方法
无。 
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **userSource 的用户**。|
|createdDateTime|DateTimeOffset|用户 **源** 的创建日期和时间|
|displayName|String|与邮箱和网站关联的显示名称。|
|email|字符串|用户邮箱的电子邮件地址。|
|id|String|**userSource** 的 ID。 这不是实际组的 ID|
|includedSources|字符串|指定此组中包含的源。 可取值为：`mailbox`、`site`。|
|siteWebUrl|String|用户 OneDrive for Business 网站的 URL。 只读。|
|holdStatus|String|**userSource** 的保留状态。可能的值为： `notApplied`， `applied`， `applying`， `removing``partial`|
### <a name="sourcetype-values"></a>sourceType 值

与用户相关的源类型。 默认包括邮箱和网站。

|成员|说明|
|:----|-----------|
|邮箱|表示邮箱。|
|网站|表示 OneDrive for Business 网站。|

### <a name="usersourceholdstatus-values"></a>userSourceHoldStatus 值

|名称|说明|
|:----|-----------|
|notApplied|userSource 未处于保留状态 (其中的所有源都未保留) 。|
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
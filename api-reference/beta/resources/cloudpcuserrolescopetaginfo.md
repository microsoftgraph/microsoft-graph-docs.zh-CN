---
title: cloudPcUserRoleScopeTagInfo 资源类型
description: 表示具有标识和显示名称范围标记信息。
author: ecmadao
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c070e11bb86b9a41ed5de05955a39599ee21e2f4
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507198"
---
# <a name="cloudpcuserrolescopetaginfo-resource-type"></a>cloudPcUserRoleScopeTagInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示具有标识和显示名称范围标记信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|范围标记显示名称。|
|roleScopeTagId|String|范围标记 ID。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserRoleScopeTagInfo",
  "displayName": "String",
  "roleScopeTagId": "String"
}
```

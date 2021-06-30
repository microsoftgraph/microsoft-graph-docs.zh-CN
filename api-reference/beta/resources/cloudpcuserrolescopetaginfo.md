---
title: cloudPcUserRoleScopeTagInfo 资源类型
description: 表示具有标识和显示名称范围标记信息。
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 61df383dca51ec2494eb10b745bc227bcfc5d9b8
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211213"
---
# <a name="cloudpcuserrolescopetaginfo-resource-type"></a>cloudPcUserRoleScopeTagInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示具有标识和显示名称范围标记信息。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

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
---
title: omaSetting 资源类型
description: OMA 设置定义。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fc811056217cb537cd3c02095c6551663ad5eb98
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111066"
---
# <a name="omasetting-resource-type"></a>omaSetting 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

OMA 设置定义。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|显示名称。|
|说明|String|说明。|
|omaUri|String|OMA。|
|secretReferenceValueId|String|用于查找解密密码的 ReferenceId。 此属性是只读的。|
|isEncrypted|Boolean|指示值字段是否加密。 此属性是只读的。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true
}
```




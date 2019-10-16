---
title: securityVendorInformation 资源类型
description: " subProvider = AppLocker）。"
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d7af6e0903e3d178bacdd7c86b4a2cab04285171
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536095"
---
# <a name="securityvendorinformation-resource-type"></a>securityVendorInformation 资源类型

包含有关安全产品/服务供应商、提供程序和 subprovider 的详细信息（例如，供应商 = Microsoft; provider = Windows Defender ATP; subProvider = AppLocker）。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|provider |字符串|特定提供商（产品/服务-非供应商公司）;例如，WindowsDefenderATP。|
|providerVersion|字符串|提供程序或 subprovider 的版本（如果存在），它将生成警报。 *Required*|
|subProvider|字符串|特定 subprovider （在聚合提供程序下）;例如，WindowsDefenderATP。|
|提供 |字符串|通知供应商的名称（例如，Microsoft、Dell、FireEye）。 *Required*|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: securityVendorInformation 资源类型
description: " subProvider = AppLocker) 。"
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 536ed37cfe8ba190a22ef86e190af2b171d352ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983982"
---
# <a name="securityvendorinformation-resource-type"></a>securityVendorInformation 资源类型

命名空间：microsoft.graph

包含有关安全产品/服务供应商、提供商和 subprovider 的详细信息 (例如，供应商 = Microsoft;提供程序 = Windows Defender ATP;subProvider = AppLocker) 。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|provider |String|特定提供商 (产品/服务-不提供供应商公司) ;例如，WindowsDefenderATP。|
|providerVersion|String|提供程序或 subprovider 的版本（如果存在），它将生成警报。 *Required*|
|subProvider|String|聚合提供程序) 下的特定 subprovider (;例如，WindowsDefenderATP。|
|提供 |String|通知供应商的名称 (例如，Microsoft、Dell、FireEye) 。 *Required*|


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


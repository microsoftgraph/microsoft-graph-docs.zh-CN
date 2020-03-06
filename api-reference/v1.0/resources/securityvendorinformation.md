---
title: securityVendorInformation 资源类型
description: " subProvider = AppLocker）。"
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: bb2b67892f5c1bffbc9844a7d30b9b16ea9cdf6e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533758"
---
# <a name="securityvendorinformation-resource-type"></a>securityVendorInformation 资源类型

命名空间：microsoft.graph

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

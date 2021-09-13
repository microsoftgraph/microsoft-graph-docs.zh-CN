---
title: securityVendorInformation 资源类型
description: " subProvider=AppLocker) 。"
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ed666cb4948d658dc877567bbbf31a0e6d551778
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142507"
---
# <a name="securityvendorinformation-resource-type"></a>securityVendorInformation 资源类型

命名空间：microsoft.graph

包含有关安全产品/服务供应商、提供程序和子提供程序的详细信息 (例如，vendor=Microsoft;provider=Windows Defender ATP;subProvider=AppLocker) 。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|提供程序 |String|特定提供商 (/服务 - 不是供应商公司) ;例如，WindowsDefenderATP。|
|providerVersion|String|生成警报的提供程序或子提供程序的版本（如果存在）。 *Required*|
|subProvider|String|聚合提供程序 (下的特定子) ;例如，WindowsDefenderATP.SmartScreen。|
|vendor |String|警报供应商的名称 (例如，Microsoft、Dell、FireEye) 。 *Required*|


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


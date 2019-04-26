---
title: securityVendorInformation 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: d543bf16617ed28d50d2e7082372ff2014cd24c5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343293"
---
# <a name="securityvendorinformation-resource-type"></a>securityVendorInformation 资源类型

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关安全产品/服务供应商、提供程序和 subprovider 的详细信息 (例如, 供应商 = Microsoft; provider = Windows Defender ATP; subprovider = AppLocker)。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|provider |String|特定提供商 (产品/服务-非供应商公司);例如, WindowsDefenderATP。|
|providerVersion|String|提供程序或 subprovider 的版本 (如果存在), 它将生成警报。 **必需**|
|subProvider|String|特定 subprovider (在聚合提供程序下);例如, WindowsDefenderATP。|
|提供 |String|通知供应商的名称 (例如, Microsoft、Dell、FireEye)。 **必需**|

## <a name="json-representation"></a>JSON 表示形式

folllowing 是资源的 JSON 表示形式。
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
<!--
{
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

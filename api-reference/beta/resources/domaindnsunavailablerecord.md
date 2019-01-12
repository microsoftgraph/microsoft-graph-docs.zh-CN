---
title: domainDnsUnavailableRecord 资源类型
description: 当您的域实体的导航属性**serviceConfigurationRecords**查询时，可能会返回一个或多个 DomainDnsCnameRecord、 DomainDnsMxRecord、 DomainDnsSrvRecord，和/或 DomainDnsTxtRecord 实体。 这些实体指示您必须先将添加到区域文件域的域可由 Microsoft Online Services 何种 DNS 记录。 当不可能生成此类实体时，而被返回 DomainDnsUnavailableRecord 实体。 继承自 DomainDnsRecord 实体。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99da0448d75375b84bb37c05102c1f702c222a25
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982790"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>domainDnsUnavailableRecord 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

查询[域](domain.md)实体的导航属性 **serviceConfigurationRecords** 时，可能会返回一个或多个 [DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md) 和/或 [DomainDnsTxtRecord](domaindnstxtrecord.md) 实体。这些实体指示 Microsoft Online Services 可以使用域前必须要添加到域的区域文件的 DNS 记录。无法生成这些实体时，将返回 DomainDnsUnavailableRecord 实体。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。

## <a name="methods"></a>方法
不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|String|提供返回 **DomainDnsUnavailableRecord** 实体的原因。 |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "canonicalName": "String",
  "description": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

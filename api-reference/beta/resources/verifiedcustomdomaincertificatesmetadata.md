---
title: verifiedCustomDomainCertificatesMetadata 资源类型
description: 表示通过应用程序代理发布的本地应用程序的自定义证书元数据。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c901050f3cd068f68557473587e96b5ea5f65905
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057755"
---
# <a name="verifiedcustomdomaincertificatesmetadata-resource-type"></a>verifiedCustomDomainCertificatesMetadata 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在使用应用程序代理发布本地应用程序时， [onPremisesPublishing](onpremisespublishing.md) 资源的自定义域证书元数据。 使用自定义域允许您为应用程序使用自己的域名，而不是默认域 msappproxy.net。 若要了解详细信息，请参阅 [AZURE AD 应用程序代理中的自定义域](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|expiryDate|DateTimeOffset| 自定义域证书的到期日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 |
|issueDate|DateTimeOffset| 自定义域的签发日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 |
|issuerName|String| 自定义域证书的颁发者名称。 |
|SubjectName|String| 自定义域证书的主题名称。 |
|为|String| 与自定义域证书关联的指纹。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedCustomDomainCertificatesMetadata",
  "baseType": null
}-->

```json
{
  "expiryDate": "String (timestamp)",
  "issueDate": "String (timestamp)",
  "issuerName": "String",
  "subjectName": "String",
  "thumbprint": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedCustomDomainCertificatesMetadata resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


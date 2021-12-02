---
title: 认证资源类型
description: 表示应用程序的认证详细信息。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: arpitha-dhanapathi
ms.openlocfilehash: 6dedb9b58e3b59c707c6601fea12e9751ec3026f
ms.sourcegitcommit: 3e2239e60b6dc53997b7d4356a20fc3d365d6238
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2021
ms.locfileid: "61266424"
---
# <a name="certification-resource-type"></a>认证资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示应用程序的认证 [详细信息](application.md)。 

应用程序的认证属性是只读的，不能手动设置。 当通过应用合规性计划对应用程序进行Microsoft 365更新。 有关详细信息，请参阅应用Microsoft 365[计划](/microsoft-365-app-certification/docs/enterprise-app-certification-guide)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---------------|:--------|:----------|
|certificationDetailsUrl|String|显示应用程序的认证详细信息的 URL。|
|certificationExpirationDateTime|DateTimeOffset|应用程序的当前认证将过期的时间戳。|
|isCertifiedByMicrosoft|布尔值|指示应用程序是否经过 Microsoft 认证。|
|isPublisherAttested|布尔值|指示应用程序是否由应用程序开发人员或发布者自行证明。|
|lastCertificationDateTime|DateTimeOffset|最近添加或更新应用程序的认证时间戳。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certification"
}-->

```json
{
  "isPublisherAttested": "Boolean",
  "isCertifiedByMicrosoft": "Boolean",
  "certificationDetailsUrl": "String",
  "lastCertificationDateTime": "DateTimeOffset",
  "certificationExpirationDateTime": "DateTimeOffset"
}
```

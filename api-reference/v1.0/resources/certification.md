---
title: 认证资源类型
description: 表示应用程序的认证详细信息。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: arpitha-dhanapathi
ms.openlocfilehash: 228670677eb8d618803bb86594a3cd95cf3f2e0d
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096321"
---
# <a name="certification-resource-type"></a>认证资源类型
命名空间：microsoft.graph

表示 [应用程序](application.md)的认证详细信息。 

应用程序的认证属性是只读的，不能手动设置。 当应用程序通过Microsoft 365应用符合性计划进行认证时，会更新该应用程序。 有关详细信息，请参阅[Microsoft 365应用符合性计划](/microsoft-365-app-certification/docs/enterprise-app-certification-guide)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---------------|:--------|:----------|
|certificationDetailsUrl|String|显示应用程序认证详细信息的 URL。|
|certificationExpirationDateTime|DateTimeOffset|应用程序当前认证到期的时间戳。|
|isCertifiedByMicrosoft|布尔值|指示应用程序是否已通过 Microsoft 认证。|
|isPublisherAttested|Boolean|指示应用程序开发人员还是发布者已自行证明应用程序。|
|lastCertificationDateTime|DateTimeOffset|最近添加或更新应用程序认证的时间戳。|

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

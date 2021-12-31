---
title: appConsentApprovalRoute 资源类型
description: 公开应用许可请求 API 和功能的基本资源的容器。 当前仅公开 appConsentRequests 关系。
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cb5e5c3c060c255d7c5154494cc0226031665e5f
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650943"
---
# <a name="appconsentapprovalroute-resource-type"></a>appConsentApprovalRoute 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

公开应用许可请求 API 和功能的基本资源的容器。 当前仅公开 [appConsentRequests](appconsentrequest.md) 关系。

继承自 [实体](entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|appConsentRequests|[appConsentRequest](../resources/appconsentrequest.md) 集合| 特定应用程序的 [userConsentRequest](../resources/userconsentrequest.md) 对象的集合。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appConsentApprovalRoute",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConsentApprovalRoute"
}
```


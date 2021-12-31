---
title: termsOfUseContainer 资源类型
description: 公开使用条款 API 及其功能的关系容器。 目前公开协议和 agreementAcceptances 关系。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: bef1033ceea7056d52586054f4ba32f98953cbe0
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651696"
---
# <a name="termsofusecontainer-resource-type"></a>termsOfUseContainer 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

公开使用条款 API 及其功能的关系容器。 目前公开 [协议和](agreement.md) [agreementAcceptances](agreementacceptance.md) 关系。

继承自 [实体](entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|agreementAcceptances|[agreementAcceptance](agreementacceptance.md) 集合| 表示用户对公司可自定义使用条款协议的响应的当前状态。|
|协议|[协议](agreement.md) 集合|表示租户的可自定义使用条款协议，该协议是使用 Azure Active Directory (Azure AD) 。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsOfUseContainer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsOfUseContainer"
}
```


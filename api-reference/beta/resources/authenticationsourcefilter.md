---
title: authenticationSourceFilter 资源类型
description: 基于用于确定是否执行侦听器的身份验证源进行筛选。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 53f765f998dffdce5dcfd549177ebd1250cf013f
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508010"
---
# <a name="authenticationsourcefilter-resource-type"></a>authenticationSourceFilter 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

基于用于确定是否评估侦听器的身份验证源进行筛选。

**includeApplications** 属性可用于在应用程序中启用自助Azure Active Directory。 有关详细信息，请参阅我们的文档，了解如何在自助服务注册用户流 [中启用应用程序](/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow)。

## <a name="properties"></a>属性

|属性|类型|Description|
|:---|:---|:---|
|includeApplications|String collection|要包含用于评估 [authenticationListener 的应用程序](../resources/authenticationlistener.md)。 当在身份验证流中用作客户端应用程序时，这些应用程序将触发关联的操作。 应用程序标识是应用程序的客户端 ID。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationSourceFilter"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.authenticationSourceFilter",
  "includeApplications": [
    "String"
  ]
}
```

---
title: authenticationSourceFilter 资源类型
description: 基于用于确定是否执行侦听器的身份验证源进行筛选。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4736be415faab65c6ce3b572a1273a73c707ee43
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128629"
---
# <a name="authenticationsourcefilter-resource-type"></a>authenticationSourceFilter 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

基于用于确定是否评估侦听器的身份验证源进行筛选。

**includeApplications** 属性可用于在 Azure Active Directory 中启用应用程序的自助注册。 阅读我们的文档以在自助服务注册用户流中启用 [应用程序，了解更多信息](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|includeApplications|字符串集合|要包含用于评估 [authenticationListener 的应用程序](../resources/authenticationlistener.md)。 当在身份验证流中用作客户端应用程序时，这些应用程序将触发关联的操作。 应用程序标识是应用程序的客户端 ID。|

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

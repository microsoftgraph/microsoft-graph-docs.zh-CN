---
title: invokeUserFlowListener 资源类型
description: 用于在身份验证事件期间调用用户流的侦听器。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0ca1c61d830a2ff98f2d72839129d75cc6287c36
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720153"
---
# <a name="invokeuserflowlistener-resource-type"></a>invokeUserFlowListener 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

你可以为[onSignUpStart 事件创建 invokeUserFlowListener。](../resources/invokeuserflowlistener.md) 这会将应用程序与用户流关联，从而启用应用程序的外部 [标识自助注册](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) 。 将应用程序与用户流关联后，转到该应用程序的用户将能够启动设置来宾帐户的注册流。

继承自抽象基类型 [authenticationListener](../resources/authenticationlistener.md)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|操作标识符。 继承自 [authenticationListener](../resources/authenticationlistener.md)。|
|priority|Int32|用于确定多个适用操作之一的操作的优先级。 继承自 [authenticationListener](../resources/authenticationlistener.md)。|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|基于用于确定是否执行侦听器的身份验证源进行筛选。 继承自 [authenticationListener](../resources/authenticationlistener.md)。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|userFlow|[b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)|执行此操作时调用的用户流。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.invokeUserFlowListener",
  "baseType": "microsoft.graph.authenticationListener",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "priority": "Integer",
  "sourceFilter": {
    "@odata.type": "microsoft.graph.authenticationSourceFilter"
  },
  "userFlow": {
    "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
  }
}
```

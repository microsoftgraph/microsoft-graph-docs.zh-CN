---
title: authenticationListener 资源类型
description: 定义在身份验证事件期间要评估的侦听器。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a7feeabaa9caf0246a53aded7ac1c15236fdf8af
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433178"
---
# <a name="authenticationlistener-resource-type"></a>authenticationListener 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义在身份验证体验中发生身份验证事件时要评估的侦听器。 authenticationListener 是抽象的，是可在身份验证事件期间评估的各种类型的侦听器的基类。 

你可以为[onSignUpStart 事件创建 invokeUserFlowListener。](../resources/invokeuserflowlistener.md) 这会将应用程序与用户流关联，从而启用自助服务 [注册](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) 过程。 将应用程序与用户流关联后，转到该应用程序的用户将能够启动设置来宾帐户的注册流。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 onSignUpStart](../api/authenticationeventspolicy-list-onsignupstart.md)|[authenticationListener](../resources/authenticationlistener.md) 集合|获取 onSignupStart 事件支持的 authenticationListener 资源的集合。|
|[创建 authenticationListener](../api/authenticationeventspolicy-post-onsignupstart.md)|[authenticationListener](../resources/authenticationlistener.md)|为 onSignupStart 事件创建新的 authenticationListener 对象。|
|[更新 authenticationListener](../api/authenticationlistener-update.md)|[authenticationListener](../resources/authenticationlistener.md)|更新为身份验证管道中的 onSignupStart 事件定义的指定侦听器。|
|[Put authenticationListener](../api/authenticationlistener-put.md)|[authenticationListener](../resources/authenticationlistener.md)|替换 authenticationListener 对象的属性。|
|[获取 authenticationListener](../api/authenticationlistener-get.md)|[authenticationListener](../resources/authenticationlistener.md)|获取为身份验证管道中的 onSignupStart 事件定义的指定侦听器。|
|[删除 authenticationListener](../api/authenticationlistener-delete.md)|无|删除为身份验证管道中的 onSignupStart 事件定义的指定侦听器。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|操作标识符。|
|priority|Int32|侦听器的优先级。 确定事件具有多个侦听器时的评估顺序。 优先级从低到高计算。|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|基于用于确定是否评估侦听器的身份验证源的筛选器。 这当前仅限于基于用户进行身份验证的应用程序的评估。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationListener",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "priority": "Integer",
  "sourceFilter": {
    "@odata.type": "microsoft.graph.authenticationSourceFilter"
  }
}
```

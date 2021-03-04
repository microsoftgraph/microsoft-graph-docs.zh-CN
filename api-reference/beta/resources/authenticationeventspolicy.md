---
title: authenticationEventsPolicy 资源类型
description: 身份验证事件用于在身份验证流中的特定点调用用户流。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6cd727ebe51bbb6d5ad2162b180c4fc891ff792a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443165"
---
# <a name="authenticationeventspolicy-resource-type"></a>authenticationEventsPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个指定身份验证体验中的事件的资源，每个事件进一步定义了为事件创建的可用侦听器类型。 事件是身份验证体验的固有特征;此资源不可用户配置。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 onSignUpStart 侦听器](../api/authenticationeventspolicy-list-onsignupstart.md)|[authenticationListener](../resources/authenticationlistener.md) 集合|获取 onSignupStart 事件支持的 authenticationListener 资源的集合。|
|[创建 authenticationListener](../api/authenticationeventspolicy-post-onsignupstart.md)|[authenticationListener](../resources/authenticationlistener.md)|为 onSignupStart 事件创建新的 authenticationListener 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|策略的标识符。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|onSignupStart|[authenticationListener](../resources/authenticationlistener.md) 集合|注册时要采取的适用操作的列表。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationEventsPolicy",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.authenticationEventsPolicy",
  "id": "String (identifier)"
}
```

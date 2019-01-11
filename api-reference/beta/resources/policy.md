---
title: 策略资源类型
description: 表示 Azure AD 策略。 策略是可以在应用程序、 服务主体、 组或分配给他们的整个组织强制实施的自定义规则。 当前只有一种类型的策略有：
localization_priority: Normal
ms.openlocfilehash: cc82dc32056b9da5c2ca1144e58b5b9e1fe326f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830924"
---
# <a name="policy-resource-type"></a>策略资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示 Azure AD 策略。 策略是可以在应用程序、 服务主体、 组或分配给他们的整个组织强制实施的自定义规则。 当前只有一种类型的策略有：

- 令牌生存期策略-指定的应用程序和服务主体颁发的令牌生存期持续时间。

进一步下面将详细介绍了此策略。

## <a name="methods"></a>方法
| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
| [获取策略](../api/policy-get.md) |策略|读取 user 对象的属性和关系。|
|[创建策略](../api/policy-post.md)|策略|创建新策略对象。|
|[更新策略](../api/policy-update.md)|无|更新策略对象。|
|[删除策略](../api/policy-delete.md)|无|删除策略对象。|
|[分配策略](../api/policy-assign.md)|无|将策略分配给应用程序，服务主体。|
|[列表策略](../api/policy-list.md)|策略集合|获取组织中的所有策略对象。|
|[列表分配策略](../api/policy-list-assigned.md)|策略集合|获取所有策略对象分配给应用程序或服务主体。|

### <a name="common-properties"></a>通用属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|definition|字符串|字符串版本的特定的策略。 请参阅下文。 必需。|
|displayName|字符串|自定义策略名称。 必填。|
|IsOrganizationDefault|布尔|如果设置为 true 时，激活此策略。 可以有多个策略相同的策略类型，但只有一个可激活为默认组织。 可选，默认值为 false。|
|type|字符串|指定策略的类型。 必须当前"TokenLifetimePolicy"。 必填。|

#### <a name="common-relationships"></a>常见的关系
|关系|类型|说明|
|:-------------|:-----------|:-----------|
|appliesTo|[directoryObject](../resources/directoryobject.md) 集合|应用程序、 服务主体、 组或组织的策略应用于。|

## <a name="token-lifetime-policy"></a>令牌生存期策略
指定针对不同目的颁发的令牌生存期。 这种策略可向应用程序和服务主体的[分配](../api/policy-assign.md)。 有四种类型的可配置其生命周期的令牌。 访问/刷新令牌对是通过客户端，身份验证过程中获得的而 ID/会话令牌对通过浏览器的身份验证过程中获得。

- **访问令牌**包含信息的标识和相关联的客户端用于访问类似于应用程序的受保护的资源的用户帐户的权限。
- **刷新令牌**获取访问令牌以及当通过客户端访问受保护的资源的 Azure AD 对用户进行身份验证。 未吊销或离开未使用的 （见下文） MaxInactiveTime 超过时, 可用于获取新的访问/刷新令牌对当前存取令牌过期时。
- **ID 令牌**像访问令牌，但通过浏览器获取。
- **会话令牌**的行为类似刷新令牌，但通过浏览器获取。

## <a name="properties"></a>属性
下列属性窗体的 JSON 对象表示的令牌生存期策略。 此 JSON 对象必须是**转换为带引号它们进行转义字符串**要插入的"定义"常见策略属性。 示例如下所示。

>注意： 所有这些属性中的持续时间格式"dd.hh:mm:ss"中指定。

>注意： 在"工作日"表示的属性的最大值是 1 秒缺少表示天数。 例如，1 天的最大值指定为"23: 59:59"。

| 属性     | 类型   |Description| 最小值 | 最大值 | 默认值|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|字符串|控制长**访问和 ID 令牌**视为有效。|10 分钟|1 天|1 小时|
|MaxInactiveTime|字符串|控制如何旧刷新令牌可之前客户端不能再使用它以检索新的访问/刷新令牌对以访问资源。|10 分钟|90 天|14 天|
|MaxAgeSingleFactor|字符串|控件长用户可以继续使用刷新令牌获取新的 access 刷新令牌对上次他们过身份验证之后成功单个因子。 由于单因素被看作安全性低于多因素身份验证，建议您使用此策略设置为比 MultiFactorRefreshTokenMaxAge 相同或更低值。|10 分钟|直到吊销|365 天或直到吊销|
|MaxAgeMultiFactor|字符串|控件长用户可以继续使用刷新令牌获取新的 access 刷新令牌对上次他们过身份验证之后成功与多因素。|10 分钟|直到吊销|365 天或直到吊销|
|MaxAgeSessionSingleFactor|字符串|控件长用户可以继续使用会话令牌获取新 ID/会话令牌之后上次他们过身份验证成功单个因子。 由于一元被视为安全性低于多因素身份验证，因此建议此策略设置为比 MultiFactorSessionTokenMaxAge 相同或更低值|10 分钟|直到吊销|365 或直到吊销|
|MaxAgeSessionMultiFactor|字符串|控件长用户可以继续使用会话令牌获取的上次成功与多因素验证之后的新 ID/会话令牌。|10 分钟|直到吊销|365 或直到吊销|
|版本|整数|设置值为 1。 必填。|无|无|无|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

```json
{
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
  "displayName":"Test Policy",
  "isOrganizationDefault":false,
  "type":"TokenLifetimePolicy",
}
```

---
title: temporaryAccessPassAuthenticationMethodConfiguration 资源类型
description: 表示临时访问传递身份验证方法策略。
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9edb4038180a96d6878fcaf6770728a1befbca19
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272601"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a>temporaryAccessPassAuthenticationMethodConfiguration 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示临时访问传递身份验证方法策略。 身份验证方法策略定义配置设置以及允许使用身份验证方法的用户或组。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|读取 **temporaryaccesspassauthenticationmethodconfiguration** 对象的属性和关系。|
|[更新](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|更新 **temporaryaccesspassauthenticationmethodconfiguration 对象** 的属性。|
|[删除](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|无|将 **temporaryaccesspassauthenticationmethodconfiguration** 对象还原到其默认配置。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法策略标识符。|
|minimumLifetimeInMinutes|Int|在租户中创建的任何 temporaryAccessPass 的最小生存期（分钟）。 值可以介于 10 到 43200 (等于 30 天) 。|
|maximumLifetimeInMinutes|Int|在租户中创建的任何 temporaryAccessPass 的最大生存期（分钟）。 值可以介于 10 到 43200 (等于 30 天) 。|
|defaultLifetimeInMinutes|int|临时AccessPass 的默认生存期（分钟）。 值可以在 minimumLifetimeInMinutes 和 maximumLifetimeInMinutes 之间。|
|defaultLength|int|temporaryAccessPass 的默认长度（以字符表示）介于 8 到 48 个字符之间。|
|isUsableOnce|布尔值   |如果 `true` ，租户中所有通道将限制为一次使用。 If `false` ， passes in the tenant can be created to be one-time use or multiple time use.|
|state|authenticationMethodState|可取值为：`enabled`、`disabled`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|includeTargets|[authenticationMethodTarget](../resources/authenticationmethodtarget.md) 集合|允许使用身份验证方法的用户或组的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

``` json
{
  "@odata.type": "#microsoft.authMethodPolicy.temporaryAccessPassAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "defaultLifetimeInMinutes": "Integer",
  "defaultLength": "Integer",
  "minimumLifetimeInMinutes": "Integer",
  "maximumLifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean"
},
"includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```

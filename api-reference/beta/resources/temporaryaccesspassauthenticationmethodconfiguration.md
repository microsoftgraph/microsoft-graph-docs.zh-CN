---
title: temporaryAccessPassAuthenticationMethodConfiguration 资源类型
description: 代表"临时访问传递身份验证方法"策略。
author: inbarckms
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 5cac99576931ff15636df6f69b548ecfb53c01f3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052542"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a>temporaryAccessPassAuthenticationMethodConfiguration 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表"临时访问传递身份验证方法"策略。 身份验证方法策略定义配置设置以及允许使用身份验证方法的用户或组。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|读取 **temporaryaccesspassauthenticationmethodconfiguration** 对象的属性和关系。|
|[更新](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|更新 **temporaryaccesspassauthenticationmethodconfiguration 对象** 的属性。|
|[删除](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|无|将 **temporaryaccesspassauthenticationmethodconfiguration** 对象还原到其默认配置。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法策略标识符。|
|minimumLifetimeInMinutes|Int|租户中创建的任何 temporaryAccessPass 的最小生存期（分钟）。 值可以介于 10 到 43200 分钟之间 (30 天) 。|
|maximumLifetimeInMinutes|Int|租户中创建的任何 temporaryAccessPass 的最大生存期（分钟）。 值可以介于 10 到 43200 分钟之间 (30 天) 。|
|defaultLifetimeInMinutes|int|temporaryAccessPass 的默认生存期（分钟）。 值可以介于 minimumLifetimeInMinutes 和 maximumLifetimeInMinutes 之间。|
|defaultLength|int|temporaryAccessPass 的默认长度（以字符表示）介于 8 到 48 个字符之间。|
|isUsableOnce|布尔值   |如果 `true` 为 ，租户中所有通道将限制为一次使用。 如果 `false` 为 ，则传递租户可创建为一次使用或多次使用。|
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

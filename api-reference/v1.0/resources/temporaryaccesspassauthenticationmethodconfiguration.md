---
title: temporaryAccessPassAuthenticationMethodConfiguration 资源类型
description: 表示临时访问传递身份验证方法策略，该策略定义配置设置以及启用了使用身份验证方法的用户或组。
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 00a797efd68cefe8daf96e46a2d4b92f265bd488
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971663"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a>temporaryAccessPassAuthenticationMethodConfiguration 资源类型
命名空间：microsoft.graph

表示临时访问传递身份验证方法策略，该策略定义配置设置以及启用了使用身份验证方法的用户或组。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|读取 **temporaryAccessPassAuthenticationMethodConfiguration** 对象的属性和关系。|
|[更新](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|无|更新 **temporaryAccessPassAuthenticationMethodConfiguration 对象的** 属性。|
|[删除](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|无|将 **temporaryAccessPassAuthenticationMethodConfiguration** 对象还原为其默认配置。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|defaultLength|Int|临时AccessPass 的默认长度（以字符为单位）。 必须介于 8 到 48 个字符之间。|
|defaultLifetimeInMinutes|Int|临时AccessPass的默认生存期（以分钟为单位）。 值可以是 **minimumLifetimeInMinutes** 和 **maximumLifetimeInMinutes** 之间的任何整数。|
|id|String|身份验证方法策略的标识符。 继承自 [entity](entity.md)。|
|isUsableOnce|布尔值   |如果 `true`是，租户中的所有传递将限制为一次性使用。 如果 `false`可以创建租户中的传递，以便一次性使用或可重用。|
|minimumLifetimeInMinutes|Int|在租户中创建的任何临时AccessPass 的最小生存期（以分钟为单位）。 值可以介于 10 到 43200 分钟之间 (等效于 30 天) 。|
|maximumLifetimeInMinutes|Int|在租户中创建的任何临时AccessPass的最大生存期（以分钟为单位）。 值可以介于 10 到 43200 分钟之间 (等效于 30 天) 。|
|state|authenticationMethodState|是否在租户中启用临时访问传递方法。 可取值为：`enabled`、`disabled`。 继承自 [authenticationMethodConfiguration](authenticationmethodconfiguration.md)。 |

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|includeTargets|[authenticationMethodTarget](../resources/authenticationmethodtarget.md) 集合|启用了使用身份验证方法的用户或组的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "defaultLifetimeInMinutes": "Integer",
  "defaultLength": "Integer",
  "minimumLifetimeInMinutes": "Integer",
  "maximumLifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```

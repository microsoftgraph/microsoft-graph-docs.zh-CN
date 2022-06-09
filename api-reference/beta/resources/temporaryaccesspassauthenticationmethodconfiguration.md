---
title: temporaryAccessPassAuthenticationMethodConfiguration 资源类型
description: 表示临时访问传递身份验证方法策略。
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 073e89cccf4f63760bcf7bcc79a28c4a0c6f7e58
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971201"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a>temporaryAccessPassAuthenticationMethodConfiguration 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示临时访问传递身份验证方法策略。 身份验证方法策略定义配置设置以及启用了使用身份验证方法的用户或组。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|读取 **temporaryaccesspassauthenticationmethodconfiguration** 对象的属性和关系。|
|[更新](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|更新 **temporaryaccesspassauthenticationmethodconfiguration** 对象的属性。|
|[删除](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|无|将 **temporaryaccesspassauthenticationmethodconfiguration** 对象还原为其默认配置。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法策略标识符。|
|minimumLifetimeInMinutes|Int|在租户中创建的任何临时AccessPass 的最小生存期（以分钟为单位）。 值可以介于 10 到 43200 分钟之间 (等效于 30 天) 。|
|maximumLifetimeInMinutes|Int|在租户中创建的任何临时AccessPass的最大生存期（以分钟为单位）。 值可以介于 10 到 43200 分钟之间 (等效于 30 天) 。|
|defaultLifetimeInMinutes|int|临时AccessPass 的默认生存期（以分钟为单位）。 值可以介于 minimumLifetimeInMinutes 和 maximumLifetimeInMinutes 之间。|
|defaultLength|int|临时AccessPass的默认长度（以字符为单位）在 8 到 48 个字符之间。|
|isUsableOnce|布尔值   |如果 `true`是，租户中的所有传递将限制为一次性使用。 如果 `false`可以创建租户中的传递，以便一次性使用或多次使用。|
|state|authenticationMethodState|可取值为：`enabled`、`disabled`。|

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
  "isUsableOnce": "Boolean"
}
```

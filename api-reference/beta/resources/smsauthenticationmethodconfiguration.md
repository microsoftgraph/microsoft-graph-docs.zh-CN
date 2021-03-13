---
title: smsAuthenticationMethodConfiguration 资源类型
description: 代表"短信身份验证方法"策略。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c5a5e62e17e5b2e1cbc96ed96a44a0c483db981d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761035"
---
# <a name="smsauthenticationmethodconfiguration-resource-type"></a>smsAuthenticationMethodConfiguration 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表"短信身份验证方法"策略。 身份验证方法策略定义配置设置以及允许使用身份验证方法的用户或组。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[Get](../api/smsauthenticationmethodconfiguration-get.md)|[smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md)|读取 smsAuthenticationMethodConfiguration 对象的属性和关系。|
|[更新](../api/smsauthenticationmethodconfiguration-update.md)|[smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md)|更新 smsAuthenticationMethodConfiguration 对象的属性。|
|[删除](../api/smsauthenticationmethodconfiguration-delete.md)|无|将 smsAuthenticationMethodConfiguration 对象还原到其默认配置。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法策略标识符。|
|state|authenticationMethodState|可取值为：`enabled`、`disabled`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|includeTargets|[smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md) 集合|允许使用身份验证方法的用户或组的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.smsAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```


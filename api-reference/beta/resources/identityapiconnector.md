---
title: identityApiConnector 资源类型
description: 表示 Azure Active Directory 租户中的 API 连接器。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7ecb96a9ca2f4397c1f0ee52908a7802374df0f
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508083"
---
# <a name="identityapiconnector-resource-type"></a>identityApiConnector 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure AD 租户和 Azure AD (Azure AD) Azure Active Directory 中的 API 连接器。

Azure AD 外部标识自助注册中使用的 API 连接器和 Azure AD B2C 注册用户流允许你在执行用户流期间调用 API。 API 连接器提供调用 API 时需要的信息，包括终结点 URL 和身份验证。 API 连接器可在用户流中的特定步骤使用，以影响用户流的执行。 例如，API 响应可以阻止用户注册、显示输入验证错误或覆盖用户收集的属性。

使用 [b2xIdentityUserFlow](b2xidentityuserflow.md) API 从外部标识自助注册用户流使用 API 连接器。

## <a name="methods"></a>方法

|方法|返回类型|Description|
|:---|:---|:---|
|[List](../api/identityapiconnector-list.md)|[identityApiConnector](identityapiconnector.md) 集合| 获取 API 连接器列表|
|[创建](../api/identityapiconnector-create.md)|[identityApiConnector](identityapiconnector.md)|创建新的 API 连接器。 |
|[获取](../api/identityapiconnector-get.md)|[identityApiConnector](identityapiconnector.md)|读取 [identityApiConnector 对象](../resources/identityapiconnector.md) 的属性。|
|[更新](../api/identityapiconnector-update.md)|[identityApiConnector](identityapiconnector.md)|更新 API 连接器的属性。|
|[上载客户端证书](../api/identityapiconnector-uploadclientcertificate.md)|[identityApiConnector](identityapiconnector.md)|上载客户端证书以用于身份验证。|
|[删除](../api/identityapiconnector-delete.md)|无|删除 API 连接器。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|API 连接器的随机生成的 ID。 |
|displayName|字符串| API 连接器的名称。 |
|targetUrl|字符串| 要调用的 API 终结点的 URL。 |
|authenticationConfiguration|[apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)|描述用于调用 API 的身份验证配置详细信息的对象。 支持基本证书和 PKCS 12 客户端证书。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityApiConnector",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityApiConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "targetUrl": "String",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
  }
}
```

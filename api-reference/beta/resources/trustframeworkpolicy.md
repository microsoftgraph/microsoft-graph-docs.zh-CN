---
title: trustFrameworkPolicy
description: 在 Azure AD B2C 信任框架策略中称为自定义策略。 这描述租户的 trustFrameworkPolicy 对象上可用的操作。
ms.localizationpriority: medium
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2f84f1ef4c391c81a720d5f0f76adae144e04677
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59100517"
---
# <a name="trustframeworkpolicy-resource-type"></a>trustFrameworkPolicy 资源类型

命名空间：microsoft.graph

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示信任[框架](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom)策略[ (B2C](/azure/active-directory-b2c/active-directory-b2c-overview)中[也称为) ](/azure/active-directory-b2c/active-directory-b2c-overview-custom)策略Azure Active Directory策略。 信任框架策略可完全控制用户旅程。 使用它：

* 完全自定义注册和登录体验。
* 联合到任何 SAML、开放 ID 连接或 OAuth2 标识提供程序。
* 通过调用 REST 终结点与其他系统或用户数据存储集成。
* 转换声明并自定义颁发给信赖方应用程序的令牌。

有关详细信息，请参阅[B2C 中的Azure Active Directory策略](/azure/active-directory-b2c/active-directory-b2c-overview-custom)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建 trustFrameworkPolicy](../api/trustframework-post-trustframeworkpolicy.md)|trustFrameworkPolicy|创建新的 trustFrameworkPolicy。|
|[获取 trustFrameworkPolicy](../api/trustframeworkpolicy-get.md) |trustFrameworkPolicy|读取现有 trustFrameworkPolicy 的属性。|
|[列出 trustFrameworkPolicies](../api/trustframework-list-trustframeworkpolicies.md)|trustFrameworkPolicy 集合|列出在租户中配置的所有 trustFrameworkPolicies。|
|[更新或创建 trustFrameworkPolicy](../api/trustframework-put-trustframeworkpolicy.md)|无|更新现有的 trustFrameworkPolicy。|
|[删除 trustFrameworkPolicy](../api/trustframeworkpolicy-delete.md)|无|删除现有的 trustFrameworkPolicy。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|id|String|策略的 ID。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType":"microsoft.graph.entity",
  "keyProperty":"id",
  "isMediaEntity":true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
}-->
```json
{
   "id": "B2C_1A_Test"
}
```

## <a name="see-also"></a>另请参阅

- [有关架构元素的信息，请参阅 trustFrameworkPolicy](/azure/active-directory-b2c/trustframeworkpolicy) 架构。
- [trustFrameworkPolicy.xsd](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)



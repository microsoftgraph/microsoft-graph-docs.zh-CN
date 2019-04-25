---
title: trustFrameworkPolicy
description: 在 Azure AD B2C 信任框架策略中称为 "自定义策略"。 这描述了适用于租户的 trustFrameworkPolicy 对象的操作。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8b822f1b9788d0502c1376ed437593dfb96469ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522620"
---
# <a name="trustframeworkpolicy-resource-type"></a>trustFrameworkPolicy 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示[Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview)中的[信任框架](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom)策略 (也称为[自定义策略](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom))。 信任框架策略提供了对用户旅程的完全控制权限。 使用它可以执行以下操作:

* 完全自定义注册和登录体验。
* 联合任何 SAML、Open ID Connect 或 OAuth2 identity provider。
* 通过调用 REST 终结点与其他系统或用户数据存储集成。
* 转换声明并自定义颁发给信赖方应用程序的令牌。

有关详细信息, 请参阅[Azure Active Directory B2C 中的自定义策略](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建 trustFrameworkPolicy](../api/trustframework-post-trustframeworkpolicy.md)|trustFrameworkPolicy|创建新的 trustFrameworkPolicy。|
|[获取 trustFrameworkPolicy](../api/trustframeworkpolicy-get.md) |trustFrameworkPolicy|读取现有 trustFrameworkPolicy 的属性。|
|[列出 trustFrameworkPolicies](../api/trustframework-list-trustframeworkpolicies.md)|trustFrameworkPolicy 集合|列出租户中配置的所有 trustFrameworkPolicies。|
|[更新或创建 trustFrameworkPolicy](../api/trustframework-put-trustframeworkpolicy.md)|无|更新现有的 trustFrameworkPolicy。|
|[删除 trustFrameworkPolicy](../api/trustframeworkpolicy-delete.md)|无|删除现有的 trustFrameworkPolicy。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|id|String|策略的 ID。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

```json
{
   "id": "B2C_1A_Test"
}
```

## <a name="see-also"></a>另请参阅

- [trustFrameworkPolicy 架构](https://docs.microsoft.com/en-us/azure/active-directory-b2c/trustframeworkpolicy), 以了解有关架构元素的信息。  
- [trustFrameworkPolicy](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)

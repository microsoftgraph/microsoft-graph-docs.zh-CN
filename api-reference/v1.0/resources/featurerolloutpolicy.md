---
title: featureRolloutPolicy 资源类型
description: 表示与目录对象关联的功能推出策略。
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c655b69a588ced1777221289d41175a73c696854
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944217"
---
# <a name="featurerolloutpolicy-resource-type"></a>featureRolloutPolicy 资源类型

命名空间：microsoft.graph

表示与目录对象关联的功能推出策略。 创建功能推出策略可帮助租户管理员在为整个组织启用功能之前，通过特定组试用 Azure AD 的功能。 这将最大限度地减少影响，并帮助管理员逐步测试和推出与身份验证相关的功能。

以下是功能推出的限制：

- 每个功能最多支持 10 个组。
- **appliesTo** 字段仅支持组。
- 不支持动态组和嵌套组。

以下是当前使用此推出策略支持部署的每个功能的先决条件。

### <a name="passthrough-authentication"></a>Passthrough 身份验证

* 确定在 R2 Windows Server 2012运行 [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) 代理的服务器。确保服务器已加入域，可以使用 Active Directory 对所选用户进行身份验证，并且可以在出站端口/URL 上与 Azure AD 通信。
* [下载](https://aka.ms/getauthagent) &在服务器上安装 Microsoft Azure AD Connect 身份验证代理。
* 若要启用高可用性，请在其他服务器上安装其他身份验证代理，如下 [所述](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability)。
* 确保正确配置了 [智能锁定](/azure/active-directory/authentication/howto-password-smart-lockout) 设置。 这是为了确保你的用户本地 Active Directory 帐户不会被坏角色锁定。

### <a name="seamlesssso"></a>SeamlessSso

* 根据这些说明为 AD[林启用](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature)[SeamlessSso。](/azure/active-directory/hybrid/how-to-connect-sso)

### <a name="passwordhashsync"></a>PasswordHashSync

* 从 [Azure](/azure/active-directory/hybrid/whatis-phs)   AD Connect 中的"可选功能"页面启用 PasswordHashSync。

### <a name="emailasalternateid"></a>EmailAsAlternateId

* 将备用电子邮件与用户帐户关联。

## <a name="methods"></a>方法

| 方法                                                                         | 返回类型                                     | 说明                                                               |
|:-------------------------------------------------------------------------------|:------------------------------------------------|:--------------------------------------------------------------------------|
| [列出 featureRolloutPolicies](../api/featurerolloutpolicies-list.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | 检索 featureRolloutPolicy 对象的列表。                          |
| [获取 featureRolloutPolicy](../api/featurerolloutpolicy-get.md)                 | [featureRolloutPolicy](featurerolloutpolicy.md) | 检索 featurerolloutpolicy 对象的属性和关系。 |
| [创建 featureRolloutPolicy](../api/featurerolloutpolicies-post.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | 创建新的 featureRolloutPolicy 对象。                                 |
| [更新 featureRolloutPolicy](../api/featurerolloutpolicy-update.md)           | [featureRolloutPolicy](featurerolloutpolicy.md) | 更新 featurerolloutpolicy 对象的属性。                     |
| [删除 featureRolloutPolicy](../api/featurerolloutpolicy-delete.md)           | 无                                            | 删除 featureRolloutPolicy 对象。                                     |
| [Assign appliesTo](../api/featurerolloutpolicy-post-appliesto.md)              | [directoryObject](directoryobject.md)           | 将 directoryObject 分配给功能推出。                              |
| [Remove appliesTo](../api/featurerolloutpolicy-delete-appliesto.md)            | 无                                            | 从功能推出中删除 directoryObject。                            |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String|此功能推出策略的说明。|
|displayName|String|此功能显示名称策略的部署策略。|
|功能|stagedFeatureName| 可取值为：`passthroughAuthentication`、`seamlessSso`、`passwordHashSync`、`emailAsAlternateId`、`unknownFutureValue`。|
|id|String| 只读。|
|isAppliedToOrganization|布尔|指示是否应当将此功能推出策略应用于整个组织。|
|isEnabled|Boolean|指示是否启用功能推出。|

### <a name="stagedfeaturename-values"></a>stagedFeatureName 值 

|成员|
|:---|
|passthroughAuthentication|
|seamlessSso|
|passwordHashSync|
|emailAsAlternateId|
|unknownFutureValue|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|appliesTo|[directoryObject](directoryobject.md) 集合| 可为 NULL。 指定启用该功能的 directoryObjects 列表。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "feature": "string",
  "id": "String (identifier)",
  "isAppliedToOrganization": false,
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "featureRolloutPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



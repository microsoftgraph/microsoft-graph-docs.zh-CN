---
title: featureRolloutPolicy 资源类型
description: 表示与目录对象相关联的功能展示策略。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a5ebc5884b0fd1ccf52fca961247e610b1c8cad5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498481"
---
# <a name="featurerolloutpolicy-resource-type"></a>featureRolloutPolicy 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与目录对象相关联的功能展示策略。 创建功能展示策略可帮助租户管理员在为整个组织启用功能之前，使用特定组试点 Azure AD 的功能。 这将最大限度地减少影响并帮助管理员逐步测试和部署与身份验证相关的功能。

以下是功能展示的限制：

- 每个功能最多支持10个组。
- **AppliesTo**字段仅支持组。
- 不支持动态组和嵌套组。

对于当前只有为使用此首展策略进行展示的每项功能，以下是必备组件。

### <a name="passthrough-authentication"></a>传递身份验证

* 确定运行 Windows Server 2012 R2 或更高版本的服务器（要在其中运行[PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta)代理）的服务器。确保服务器已加入域，可以使用 Active Directory 对所选用户进行身份验证，并且可以在出站端口/Url 上与 Azure AD 进行通信。
* [下载](https://aka.ms/getauthagent)& 在服务器上安装 MICROSOFT Azure AD Connect 身份验证代理。
* 若要启用高可用性，请在其他服务器上安装其他身份验证代理[，如下所述。](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability)
* 确保您已正确配置了[智能锁定](/azure/active-directory/authentication/howto-password-smart-lockout)设置。 这是为了确保用户的本地 Active Directory 帐户不会被不良参与者锁定。

### <a name="seamlesssso"></a>SeamlessSso

* 根据[这些](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature)说明为 AD 林启用[SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) 。

### <a name="passwordhashsync"></a>PasswordHashSync

* 从 Azure AD Connect 中的 "可选功能" 页启用 [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) 。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 featureRolloutPolicies](../api/directory-list-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | 检索 featureRolloutPolicy 对象的列表。 |
| [获取 featureRolloutPolicy](../api/featurerolloutpolicy-get.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | 检索 featurerolloutpolicy 对象的属性和关系。 ||
| [创建 featureRolloutPolicy](../api/directory-post-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | 创建新的 featureRolloutPolicy 对象。
| [更新 featureRolloutPolicy](../api/featurerolloutpolicy-update.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | 更新 featurerolloutpolicy 对象的属性。 |
| [删除 featureRolloutPolicy](../api/featurerolloutpolicy-delete.md) | 无 | 删除 featureRolloutPolicy 对象。 |
| [分配 appliesTo](../api/featurerolloutpolicy-post-appliesto.md) | [directoryObject](directoryobject.md) | 将 directoryObject 分配给功能推出。 |
| [删除 appliesTo](../api/featurerolloutpolicy-delete-appliesto.md) | 无 | 从功能推出中删除 directoryObject。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String|此功能展示策略的说明。|
|displayName|String|此功能展示策略的显示名称。|
|功能|stagedFeatureName| 可取值为：`passthroughAuthentication`、`seamlessSso`、`passwordHashSync`、`unknownFutureValue`。|
|id|字符串| 只读。|
|isAppliedToOrganization|布尔|指示是否应将此功能展示策略应用于整个组织。|
|isEnabled|Boolean|指示是否启用功能展示。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|appliesTo|[directoryObject](directoryobject.md) 集合| 可为 NULL。 指定为其启用功能的 directoryObjects 列表。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "baseType": "",
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

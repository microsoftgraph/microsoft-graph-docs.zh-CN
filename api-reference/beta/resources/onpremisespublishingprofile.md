---
title: onPremisesPublishingProfile 资源类型
description: onPremisesPublishingProfile 资源类型。
ms.localizationpriority: medium
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 2d984b304b47005db4de02d920cacc37ba21fb3c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125079"
---
# <a name="onpremisespublishingprofile-resource-type"></a>onPremisesPublishingProfile 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

各种 Azure 服务 (例如，Azure Active Directory 连接[](/azure/active-directory/app-proxy/what-is-application-proxy)[Passthrough Authentication、Workday](/azure/active-directory/hybrid/how-to-connect-pta)到 Azure AD[用户](/azure/active-directory/saas-apps/workday-inbound-tutorial)预配，以及应用程序代理允许从企业网络外部访问各种本地资源。

[可以将本地](onpremisesagent.md)代理 (或由管理员安装的应用程序[](connector.md)代理) 连接器，以将请求路由到特定的[已发布资源](publishedresource.md)。
[应用程序](onpremisesagentgroup.md) (代理的代理组或[](connectorgroup.md)连接器) 使管理员能够分配特定代理来为发布的特定本地资源提供服务。 管理员还可以将多个代理分组在一起，然后将每个已发布的资源分配给代理组。 同一内部部署发布类型的整个实体集由 **onPremisesPublishingProfile 表示**。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [Get onPremisesPublishingProfile](../api/onpremisespublishingprofile-get.md) | [onPremisesPublishingProfile](onpremisespublishingprofile.md) | 读取 **onPremisesPublishingProfile 对象的属性和** 关系。 |
| [更新 onPremisesPublishingProfile](../api/onpremisespublishingprofile-update.md) | None | 更新 [onPremisesPublishingProfile](onpremisespublishingprofile.md) 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](hybridagentupdaterconfiguration.md)| 代表 **hybridAgentUpdaterConfiguration** 对象。|
|id|String| 表示发布类型。 可取值为：`applicationProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。 只读。|
|isEnabled|Boolean| 表示[Azure AD是否启用了](/azure/active-directory/app-proxy/what-is-application-proxy)租户的应用程序代理。 |

## <a name="relationships"></a>关系

| 关系 | 类型        | Description |
|:-------------|:------------|:------------|
|agentGroups|[onPremisesAgentGroup](onpremisesagentgroup.md) 集合| 现有 **onPremisesAgentGroup 对象** 的列表。 只读。 可为 NULL。|
|agents|[onPremisesAgent](onpremisesagent.md) 集合| 现有 **onPremisesAgent 对象** 的列表。 只读。 可为 NULL。|
|connectorGroups|[connectorGroup](connectorgroup.md) 集合| 通过应用程序代理发布的应用程序的现有 **connectorGroup** 对象列表。 只读。 可为 NULL。|
|连接器|[连接器](connector.md) 集合| 通过应用程序 **代理** 发布的应用程序的现有连接器对象列表。 只读。 可为 NULL。|
|publishedResources|[publishedResource](publishedresource.md) 集合| 现有 **publishedResource 对象** 的列表。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
  "keyProperty": "id"
}-->

```json
{
  "hybridAgentUpdaterConfiguration": {"@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
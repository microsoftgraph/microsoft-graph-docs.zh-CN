---
title: onPremisesPublishingProfile 资源类型
description: onPremisesPublishingProfile 资源类型。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: a7dc65f0640d2bfde9a46595b04fc24fc7512475
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156706"
---
# <a name="onpremisespublishingprofile-resource-type"></a>onPremisesPublishingProfile 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

各种 Azure (例如，Azure Active Directory Connect [Passthrough](/azure/active-directory/hybrid/how-to-connect-pta)Authentication、Workday [to Azure AD users provisioning](/azure/active-directory/saas-apps/workday-inbound-tutorial)和应用程序 [代理](https://aka.ms/whyappproxy) 允许从企业网络外部访问各种本地资源。

[可以将由](onpremisesagent.md) (安装的应用程序代理或) 连接器[](connector.md)本地代理配置为将请求路由到特定的[已发布资源](publishedresource.md)。
[通过应用程序](onpremisesagentgroup.md) (代理的代理组[](connectorgroup.md)或) 组，管理员可以分配特定代理，为发布的特定本地资源提供服务。 管理员还可以将多个代理分组在一起，然后将每个已发布的资源分配给代理组。 同一本地发布类型的整个实体集由 **onPremisesPublishingProfile 表示**。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 onPremisesPublishingProfile](../api/onpremisespublishingprofile-get.md) | [onPremisesPublishingProfile](onpremisespublishingprofile.md) | 读取 **onPremisesPublishingProfile** 对象的属性和关系。 |
| [更新 onPremisesPublishingProfile](../api/onpremisespublishingprofile-update.md) | 无 | 更新 [onPremisesPublishingProfile](onpremisespublishingprofile.md) 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](hybridagentupdaterconfiguration.md)| 代表 **hybridAgentUpdaterConfiguration** 对象。|
|id|String| 表示发布类型。 可取值为：`applicationProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。 只读。|
|isEnabled|Boolean| 表示是否 [为租户启用了 Azure AD](https://aka.ms/whyappproxy) 应用程序代理。 |

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
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




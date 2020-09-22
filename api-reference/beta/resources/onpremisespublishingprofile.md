---
title: onPremisesPublishingProfile 资源类型
description: onPremisesPublishingProfile 资源类型。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b0f2bf125593c72ba72ae4109baffcae46e88f33
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998633"
---
# <a name="onpremisespublishingprofile-resource-type"></a>onPremisesPublishingProfile 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

各种 Azure 服务 (例如，Azure Active Directory Connect [直通身份验证](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta)、从 [WORKDAY 到 azure AD 用户设置](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)以及 [应用程序代理](https://aka.ms/whyappproxy) 允许从公司网络外部访问各种本地资源。

可将[本地代理](onpremisesagent.md) (或[连接器](connector.md)，以供管理员安装的应用程序代理) 配置为将请求路由到特定的[已发布资源](publishedresource.md)。
[代理组](onpremisesagentgroup.md) (或 [连接器组](connectorgroup.md) 应用程序代理) 使管理员能够分配特定的代理来满足特定的已发布内部部署资源。 管理员还可以将多个代理组合在一起，然后将每个已发布的资源分配给一个代理组。 同一本地发布类型的整个实体集由 **onPremisesPublishingProfile**表示。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 onPremisesPublishingProfile](../api/onpremisespublishingprofile-get.md) | [onPremisesPublishingProfile](onpremisespublishingprofile.md) | 读取 **onPremisesPublishingProfile** 对象的属性和关系。 |
| [更新 onPremisesPublishingProfile](../api/onpremisespublishingprofile-update.md) | 无 | 更新 [onPremisesPublishingProfile](onpremisespublishingprofile.md) 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](hybridagentupdaterconfiguration.md)| 表示一个 **hybridAgentUpdaterConfiguration** 对象。|
|id|String| 表示发布类型。 可取值为：`applicationProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。 只读。|
|isEnabled|Boolean| 表示是否为租户启用了 [AZURE AD 应用程序代理](https://aka.ms/whyappproxy) 。 |

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|agentGroups|[onPremisesAgentGroup](onpremisesagentgroup.md) 集合| 现有 **onPremisesAgentGroup** 对象的列表。 只读。 可为 Null。|
|agent|[onPremisesAgent](onpremisesagent.md) 集合| 现有 **onPremisesAgent** 对象的列表。 只读。 可为 Null。|
|connectorGroups|[connectorGroup](connectorgroup.md) 集合| 通过应用程序代理发布的应用程序的现有 **connectorGroup** 对象的列表。 只读。 可为 Null。|
|插槽|[连接器](connector.md) 集合| 通过应用程序代理发布的应用程序的现有 **连接器** 对象的列表。 只读。 可为 Null。|
|publishedResources|[publishedResource](publishedresource.md) 集合| 现有 **publishedResource** 对象的列表。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
  "baseType": "",
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



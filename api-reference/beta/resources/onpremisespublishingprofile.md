---
title: onPremisesPublishingProfile 资源类型
description: onPremisesPublishingProfile 资源类型。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b36f8307e580bc018a713822e4e9f2ea6f5586c
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556231"
---
# <a name="onpremisespublishingprofile-resource-type"></a>onPremisesPublishingProfile 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

各种 Azure 服务（例如，Azure Active Directory Connect to [Authentication](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta)、 [WORKDAY 到 azure AD 用户预配](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)和[应用程序代理](https://aka.ms/whyappproxy)允许访问公司网络外部的各种本地资源。

可将管理员安装的[内部部署代理](onpremisesagent.md)（或应用程序代理的[连接器](connector.md)）配置为将请求路由到特定的[已发布资源](publishedresource.md)。
[代理组](onpremisesagentgroup.md)（或应用程序代理的[连接器组](connectorgroup.md)）使管理员能够分配特定的代理以满足特定的已发布内部部署资源。 管理员还可以将多个代理组合在一起，然后将每个已发布的资源分配给一个代理组。 同一本地发布类型的整个实体集由**onPremisesPublishingProfile**表示。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 onPremisesPublishingProfile](../api/onpremisespublishingprofile-get.md) | [onPremisesPublishingProfile](onpremisespublishingprofile.md) | 读取**onPremisesPublishingProfile**对象的属性和关系。 |
| [更新 onPremisesPublishingProfile](../api/onpremisespublishingprofile-update.md) | 无 | 更新[onPremisesPublishingProfile](onpremisespublishingprofile.md)对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](hybridagentupdaterconfiguration.md)| 表示一个**hybridAgentUpdaterConfiguration**对象。|
|id|String| 表示发布类型。 可取值为：`applicationProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。 只读。|
|isEnabled|Boolean| 表示是否为租户启用了[AZURE AD 应用程序代理](https://aka.ms/whyappproxy)。 |

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|agentGroups|[onPremisesAgentGroup](onpremisesagentgroup.md)集合| 现有**onPremisesAgentGroup**对象的列表。 只读。 可为 NULL。|
|agent|[onPremisesAgent](onpremisesagent.md)集合| 现有**onPremisesAgent**对象的列表。 只读。 可为 NULL。|
|connectorGroups|[connectorGroup](connectorgroup.md)集合| 通过应用程序代理发布的应用程序的现有**connectorGroup**对象的列表。 只读。 可为 NULL。|
|插槽|[连接器](connector.md)集合| 通过应用程序代理发布的应用程序的现有**连接器**对象的列表。 只读。 可为 NULL。|
|publishedResources|[publishedResource](publishedresource.md)集合| 现有**publishedResource**对象的列表。 只读。 可为 Null。|

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

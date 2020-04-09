---
title: onPremisesPublishingProfile 资源类型
description: onPremisesPublishingProfile 资源类型。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0a4e1e40a5a8774be9498f6b89d235557ba2948e
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200024"
---
# <a name="onpremisespublishingprofile-resource-type"></a>onPremisesPublishingProfile 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

各种 Azure 服务（例如，Azure Active Directory Connect 直通身份验证、从 Workday 到 Azure AD 用户预配）允许有条件访问公司网络外部的各种本地资源。 可将租户管理员安装的[本地代理](onpremisesagent.md)配置为访问/处理特定的[已发布资源](publishedresource.md)的请求。
通过[代理组](onpremisesagentgroup.md)，租户管理员可以分配特定的代理来服务特定的已发布内部部署资源。 租户管理员可以将许多代理组合在一起，然后将每个已发布的资源分配给一个组。 同一本地发布类型的整个实体集由**onPremisesPublishingProfile**表示。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 onPremisesPublishingProfile](../api/onpremisespublishingprofile-get.md) | [onPremisesPublishingProfile](onpremisespublishingprofile.md) | 读取**onPremisesPublishingProfile**对象的属性和关系。 |
| [更新 onPremisesPublishingProfile](../api/onpremisespublishingprofile-update.md) | 无 | 更新[onPremisesPublishingProfile](onpremisespublishingprofile.md)对象。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](hybridagentupdaterconfiguration.md)| 表示一个**hybridAgentUpdaterConfiguration**对象。|
|id|字符串| 表示发布类型。 可取值为：`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。 只读。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|agentGroups|[onPremisesAgentGroup](onpremisesagentgroup.md)集合| 现有**onPremisesAgentGroup**对象的列表。 此为只读属性。 可为 Null。|
|agent|[onPremisesAgent](onpremisesagent.md)集合| 已存在的**onPremisesAgent**对象的列表。 此为只读属性。 可为 Null。|
|publishedResources|[publishedResource](publishedresource.md)集合| 现有**publishedResource**对象的列表。 此为只读属性。 可为 Null。|

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

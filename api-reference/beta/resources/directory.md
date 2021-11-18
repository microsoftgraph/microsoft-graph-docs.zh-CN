---
title: 目录资源类型（已删除的项目）
description: . 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 36fbef413478ac31fa4cafbc3f30166d6e318919
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077633"
---
# <a name="directory-resource-type"></a>目录资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示目录中已删除的项目。 删除某个项目后，它会被添加到已删除项目“容器”中。 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。

目前，仅应用程序、组和用户资源支持[已删除项目功能](user.md)。 [](group.md) [](application.md)

继承自 [实体](entity.md)。

## <a name="methods"></a>Methods

| 方法         | 返回类型 | Description |
|:---------------|:------------|:------------|
|[Get deleted item](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | 获取已删除项目的属性。 |
|[Restore deleted item](../api/directory-deleteditems-restore.md) |[directoryObject](directoryobject.md)| 还原最近删除的项目。 |
|[List deleted items](../api/directory-deleteditems-list.md) |[directoryObject](directoryobject.md) 集合| 获取最近删除的项目列表。 |
|[Permanently delete an item](../api/directory-deleteditems-delete.md) | 无 | 永久删除项目。 |
|[列出用户拥有的已删除项目](../api/directory-deleteditems-user-owned.md) | [directoryObject](directoryobject.md) collection | 列出用户拥有的目录项。 |

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|String| 对象的唯一标识符;例如， `12345678-9abc-def0-1234-56789abcde` 。 键。 不可为 null。 只读。 继承自 [实体](entity.md)。|

## <a name="relationships"></a>关系

| 关系 | 类型   |Description|
|:---------------|:--------|:----------|
|administrativeUnits|[administrativeUnit](administrativeunit.md) 集合| 用户和组目录对象的概念容器。|
|attributeSets|[attributeSet](attributeset.md) 集合| 相关自定义安全属性定义的组。|
|customSecurityAttributeDefinitions|[customSecurityAttributeDefinition](customsecurityattributedefinition.md) 集合|自定义安全属性的架构 (键值对) 。|
|DeletedItems|[directoryObject](directoryobject.md) 集合| 最近删除的项目。 只读。 可为空。|
|featureRolloutPolicies|[featureRolloutPolicy](featurerolloutpolicy.md) 集合| 可为 NULL。|
|federationConfigurations|[identityProviderBase](../resources/identityproviderbase.md) 集合|配置与标识提供程序支持 IdP (组织) SAML 或 WS-Fed 联盟。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "@odata.type": "#microsoft.graph.directory"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



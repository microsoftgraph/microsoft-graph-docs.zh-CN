---
title: configManagerCollection 资源类型
description: 一个 ConfigManager 定义的设备或用户集合。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3bc7d7d371a0bbc07b29835c5ed2a4b23078cf04
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301860"
---
# <a name="configmanagercollection-resource-type"></a>configManagerCollection 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一个 ConfigManager 定义的设备或用户集合。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 configManagerCollections](../api/intune-partnerintegration-configmanagercollection-list.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 集合|列出 [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 对象的属性和关系。|
|[获取 configManagerCollection](../api/intune-partnerintegration-configmanagercollection-get.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|读取 [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 对象的属性和关系。|
|[创建 configManagerCollection](../api/intune-partnerintegration-configmanagercollection-create.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|创建新的 [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 对象。|
|[删除 configManagerCollection](../api/intune-partnerintegration-configmanagercollection-delete.md)|无|删除 [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)。|
|[更新 configManagerCollection](../api/intune-partnerintegration-configmanagercollection-update.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|更新 [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 对象的属性。|
|[getPolicySummary 函数](../api/intune-partnerintegration-configmanagercollection-getpolicysummary.md)|[configManagerPolicySummary](../resources/intune-partnerintegration-configmanagerpolicysummary.md)|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|ConfigManager 集合的键。|
|displayName|字符串|DisplayName。|
|collectionIdentifier|字符串|SCCM 中的集合标识符。|
|hierarchyName|字符串|HierarchyName。|
|hierarchyIdentifier|字符串|层次结构标识符。|
|createdDateTime|DateTimeOffset|创建日期。|
|lastModifiedDateTime|DateTimeOffset|上次修改日期。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.configManagerCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configManagerCollection",
  "id": "String (identifier)",
  "displayName": "String",
  "collectionIdentifier": "String",
  "hierarchyName": "String",
  "hierarchyIdentifier": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```





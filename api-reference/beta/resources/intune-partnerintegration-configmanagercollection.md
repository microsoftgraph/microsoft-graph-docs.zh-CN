---
title: configManagerCollection 资源类型
description: ConfigManager 定义的设备或用户集合。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d7c4300dc1cedbc316e6e8cfa5c0efebd1e383f8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033460"
---
# <a name="configmanagercollection-resource-type"></a>configManagerCollection 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ConfigManager 定义的设备或用户集合。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 configManagerCollections](../api/intune-partnerintegration-configmanagercollection-list.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 集合|列出 [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 对象的属性和关系。|
|[获取 configManagerCollection](../api/intune-partnerintegration-configmanagercollection-get.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|读取 [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 对象的属性和关系。|
|[创建 configManagerCollection](../api/intune-partnerintegration-configmanagercollection-create.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|创建新的 [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 对象。|
|[删除 configManagerCollection](../api/intune-partnerintegration-configmanagercollection-delete.md)|无|删除 [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)。|
|[更新 configManagerCollection](../api/intune-partnerintegration-configmanagercollection-update.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|更新 [configManagerCollection 对象](../resources/intune-partnerintegration-configmanagercollection.md) 的属性。|
|[getPolicySummary 函数](../api/intune-partnerintegration-configmanagercollection-getpolicysummary.md)|[configManagerPolicySummary](../resources/intune-partnerintegration-configmanagerpolicysummary.md)|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|ConfigManager 集合的键。|
|displayName|String|DisplayName。|
|collectionIdentifier|String|SCCM 中的集合标识符。|
|hierarchyName|String|HierarchyName。|
|hierarchyIdentifier|String|层次结构标识符。|
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




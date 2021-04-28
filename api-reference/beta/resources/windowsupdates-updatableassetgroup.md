---
title: updatableAssetGroup 资源类型
description: 一组可接收更新的 azureADDevice 资源。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a3aca42b69a906f167393cfd284d6756b3c4bb52
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067299"
---
# <a name="updatableassetgroup-resource-type"></a>updatableAssetGroup 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一组可接收更新的 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源。

成员为 [azureADDevice 资源](../resources/windowsupdates-azureADDevice.md) 类型。 **updatableAssetGroup** 资源不能是另一 **个 updatableAssetGroup 的成员**。

继承自 [updatableAsset](../resources/windowsupdates-updatableasset.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 updatableAssetGroup 资源](../api/windowsupdates-updates-list-updatableassets-updatableassetgroup.md)|[microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 集合|获取 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象及其属性的列表。|
|[创建 updatableAssetGroup](../api/windowsupdates-updates-post-updatableassets-updatableassetgroup.md)|[microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)|创建新的 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象。|
|[获取 updatableAssetGroup](../api/windowsupdates-updatableassetgroup-get.md)|[microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)|读取 [updatableAssetGroup 对象的属性和](../resources/windowsupdates-updatableassetgroup.md) 关系。|
|[删除 updatableAssetGroup](../api/windowsupdates-updatableassetgroup-delete.md)|无|删除 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象。|
|[添加成员](../api/windowsupdates-updatableassetgroup-addmembers.md)|无|将成员添加到 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)。|
|[按 ID (添加) ](../api/windowsupdates-updatableassetgroup-addmembers.md)|无|将成员添加到 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)。|
|[删除成员](../api/windowsupdates-updatableassetgroup-removemembers.md)|无|从 [updatableAssetGroup 中删除成员](../resources/windowsupdates-updatableassetgroup.md)。|
|[按 ID (删除) ](../api/windowsupdates-updatableassetgroup-removemembers.md)|无|从 [updatableAssetGroup 中删除成员](../resources/windowsupdates-updatableassetgroup.md)。|
|[List members](../api/windowsupdates-updatableassetgroup-list-members.md)|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|从 [members 导航属性获取 updatableAsset](../resources/windowsupdates-updatableasset.md) 资源。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|组的标识符。 键。 不可为 null。 只读。 默认情况下返回。 继承自 [updatableAsset](../resources/windowsupdates-updatableasset.md)。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|成员|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|组的成员。 只读。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetGroup",
  "baseType": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
  "id": "String (identifier)"
}
```


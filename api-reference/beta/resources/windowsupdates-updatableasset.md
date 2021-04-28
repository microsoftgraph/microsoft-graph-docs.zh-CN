---
title: updatableAsset 资源类型
description: 表示可以接收更新的资产。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 4bfdd3663c0868d22b262d398e505e0e8cb82835
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067296"
---
# <a name="updatableasset-resource-type"></a>updatableAsset 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可以接收更新的资产。

所有可更新资源作为以下派生类型之一存在 [：azureADDevice](../resources/windowsupdates-azureaddevice.md) 和 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)。

[azureADDevice 和](../resources/windowsupdates-azureaddevice.md) [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)的基本类型。

这是一个抽象类型。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 updatableAsset 资源](../api/windowsupdates-updates-list-updatableassets.md)|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|获取 [updatableAsset 对象](../resources/windowsupdates-updatableasset.md) 及其属性的列表。|
|[创建 updatableAssetGroup](../api/windowsupdates-updates-post-updatableassets-updatableassetgroup.md)|[microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)|创建新的 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象。|
|[获取 updatableAsset](../api/windowsupdates-updatableasset-get.md)|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|读取 [updatableAsset 对象的属性和](../resources/windowsupdates-updatableasset.md) 关系。|
|[删除 updatableAsset](../api/windowsupdates-updatableasset-delete.md)|无|删除 [updatableAsset](../resources/windowsupdates-updatableasset.md) 对象。|
|[在管理中注册资产](../api/windowsupdates-updatableasset-enrollassets.md)|无|在[部署服务的更新管理中注册 updatableAssets。](../resources/windowsupdates-updatableasset.md)|
|[按 ID 管理 (资产) ](../api/windowsupdates-updatableasset-enrollassetsbyid.md)|无|在部署服务更新管理中注册相同类型的[updatableAssets。](../resources/windowsupdates-updatableasset.md)|
|[从管理中注销资产](../api/windowsupdates-updatableasset-unenrollassets.md)|无|从部署服务的更新管理中注销[updatableAssets。](../resources/windowsupdates-updatableasset.md)|
|[注销按 ID 管理 (资产) ](../api/windowsupdates-updatableasset-unenrollassetsbyid.md)|无|从部署服务更新管理中注销相同类型的[updatableAssets。](../resources/windowsupdates-updatableasset.md)|
|[向组添加成员](../api/windowsupdates-updatableassetgroup-addmembers.md)|无|将成员添加到 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)。|
|[按 ID (将成员添加到) ](../api/windowsupdates-updatableassetgroup-addmembersbyid.md)|无|将相同类型的成员添加到 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)。|
|[从组中删除成员](../api/windowsupdates-updatableassetgroup-removemembers.md)|无|从 [updatableAssetGroup 中删除成员](../resources/windowsupdates-updatableassetgroup.md)。|
|[按 ID (从组中删除) ](../api/windowsupdates-updatableassetgroup-removemembersbyid.md)|无|从 [updatableAssetGroup 中删除相同类型的成员](../resources/windowsupdates-updatableassetgroup.md)。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|资产的标识符。 键。 不可为 null。 只读。 默认情况下返回。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
  "id": "String (identifier)"
}
```


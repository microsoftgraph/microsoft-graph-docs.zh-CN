---
title: taxGroups 资源类型
description: Dynamics 365 Business Central 中的税务组对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: bdfbec8f5373637924262388dab0e9c74c363af9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543124"
---
# <a name="taxgroups-resource-type"></a>taxGroups 资源类型
代表 Dynamics 365 Business Central 中的 taxGroups 资源类型。

## <a name="methods"></a>方法
| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 taxGroups](../api/dynamics-taxgroups-get.md)|taxGroups|获取税务组对象。|
|[Post taxGroups](../api/dynamics-create-taxgroups.md)|taxGroups|创建税务组对象。|
|[修补程序 taxGroups](../api/dynamics-taxgroups-update.md)|taxGroups|更新税务组对象。|
|[删除 taxGroups](../api/dynamics-taxgroups-delete.md)|无|删除税务组对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|GUID|taxGroup 的唯一 ID。 只读。|
|code|string|指定税务组。|
|displayName|string|指定税务组的显示名称。|
|taxType|string|指定组的税金类型。|
|lastModifiedDateTime|datetime|税组的最后修改日期时间。 只读。|  


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是 taxGroup 的 JSON 表示形式。

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```



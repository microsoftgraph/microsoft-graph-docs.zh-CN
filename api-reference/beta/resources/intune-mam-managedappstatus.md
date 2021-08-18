---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f437691e27d11f67a6407b9a6c510248a2b1dc2775bdb61adc28d45179804fe6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178897"
---
# <a name="managedappstatus-resource-type"></a>managedAppStatus 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示组织的应用保护和配置状态。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedAppStatuses](../api/intune-mam-managedappstatus-list.md)|[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合|列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。|
|[获取 managedAppStatus](../api/intune-mam-managedappstatus-get.md)|[managedAppStatus](../resources/intune-mam-managedappstatus.md)|读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|状态报告的友好名称。|
|id|字符串|实体的键。|
|version|String|实体的版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```





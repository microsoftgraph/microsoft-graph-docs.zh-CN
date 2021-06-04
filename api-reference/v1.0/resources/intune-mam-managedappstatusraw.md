---
title: managedAppStatusRaw 资源类型
description: 表示有关组织应用保护和配置的非类型化状态报告。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1d29ec2d96d38c6bc1f2fccf5fb5b36e16e1c5be
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752768"
---
# <a name="managedappstatusraw-resource-type"></a>managedAppStatusRaw 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示有关组织应用保护和配置的非类型化状态报告。


继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 managedAppStatusRaws](../api/intune-mam-managedappstatusraw-list.md)|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 集合|列出 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。|
|[获取 managedAppStatusRaw](../api/intune-mam-managedappstatusraw-get.md)|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)|读取 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|状态报告的友好名称。 继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)|
|id|String|实体的键。 继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)|
|version|String|实体的版本。 继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)|
|content|[Json](../resources/intune-mam-json.md)|状态报告内容。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```





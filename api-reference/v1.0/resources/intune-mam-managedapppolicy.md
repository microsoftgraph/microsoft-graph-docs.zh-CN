---
title: managedAppPolicy 资源类型
description: ManagedAppPolicy 资源表示特定于平台的策略的基类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 829e7df910bcc4e7047103f12ecd528df9f03f9f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142534"
---
# <a name="managedapppolicy-resource-type"></a>managedAppPolicy 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ManagedAppPolicy 资源表示特定于平台的策略的基类型。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedAppPolicies](../api/intune-mam-managedapppolicy-list.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合|列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。|
|[Get managedAppPolicy](../api/intune-mam-managedapppolicy-get.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|读取 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。|
|[targetApps 操作](../api/intune-mam-managedapppolicy-targetapps.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|策略显示名称。|
|说明|String|策略的说明。|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。|
|id|String|实体的键。|
|version|String|实体的版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String"
}
```





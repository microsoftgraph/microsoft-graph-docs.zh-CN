---
title: raProfileDatabaseEntity 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4a90d03258e4e84706d4828aaae2d10a1c064942
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124260"
---
# <a name="raprofiledatabaseentity-resource-type"></a>raProfileDatabaseEntity 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 raProfileDatabaseEntities](../api/intune-rapolicy-raprofiledatabaseentity-list.md)|[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)集合|列出[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)对象的属性和关系。|
|[获取 raProfileDatabaseEntity](../api/intune-rapolicy-raprofiledatabaseentity-get.md)|[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)|读取[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)对象的属性和关系。|
|[创建 raProfileDatabaseEntity](../api/intune-rapolicy-raprofiledatabaseentity-create.md)|[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)|创建新的[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)对象。|
|[删除 raProfileDatabaseEntity](../api/intune-rapolicy-raprofiledatabaseentity-delete.md)|无|删除[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)。|
|[更新 raProfileDatabaseEntity](../api/intune-rapolicy-raprofiledatabaseentity-update.md)|[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)|更新[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|version|Int32|尚未记录|
|isDeleted|Boolean|尚未记录|
|softDeletedTime|DateTimeOffset|尚未记录|
|displayName|String|尚未记录|
|linkedProfileIds|Guid 集合|尚未记录|
|profileTypeName|String|尚未记录|
|profileBody|String|尚未记录|
|profileBodyHash|String|尚未记录|
|platformType|Int32|尚未记录|
|transformedProfileBody|String|尚未记录|
|transformedProfileBodyHash|String|尚未记录|
|tenantId|Guid|尚未记录|
|profileId|Guid|尚未记录|
|eTag|String|尚未记录|
|schemaVersion|[raPolicyServiceVersions](../resources/intune-rapolicy-rapolicyserviceversions.md)|尚未记录。 可取值为：`initial`、`betaStart`、`experimentStart`、`mmpcStart`、`iosStart`。|
|lastModified|DateTimeOffset|尚未记录|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.raProfileDatabaseEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
  "version": 1024,
  "isDeleted": true,
  "softDeletedTime": "String (timestamp)",
  "displayName": "String",
  "linkedProfileIds": [
    "Guid"
  ],
  "profileTypeName": "String",
  "profileBody": "String",
  "profileBodyHash": "String",
  "platformType": 1024,
  "transformedProfileBody": "String",
  "transformedProfileBodyHash": "String",
  "tenantId": "Guid",
  "profileId": "Guid",
  "eTag": "String",
  "schemaVersion": "String",
  "lastModified": "String (timestamp)"
}
```




---
title: groupPolicyOperation 资源类型
description: 实体表示组策略操作。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad6ee2f261c14a4a1ad7548561ac6487d2745223
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086097"
---
# <a name="grouppolicyoperation-resource-type"></a>groupPolicyOperation 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体表示组策略操作。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyOperations](../api/intune-grouppolicy-grouppolicyoperation-list.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) 集合|列出 [groupPolicyOperation 对象的属性和](../resources/intune-grouppolicy-grouppolicyoperation.md) 关系。|
|[获取 groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-get.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|读取 [groupPolicyOperation 对象的属性和](../resources/intune-grouppolicy-grouppolicyoperation.md) 关系。|
|[创建 groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-create.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|创建新的 [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) 对象。|
|[删除 groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-delete.md)|无|删除 [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)。|
|[更新 groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-update.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|更新 [groupPolicyOperation 对象](../resources/intune-grouppolicy-grouppolicyoperation.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|operationType|[groupPolicyOperationType](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|组策略操作的类型。 可取值为：`none`、`upload`、`uploadNewVersion`、`addLanguageFiles`、`removeLanguageFiles`、`updateLanguageFiles` 或 `remove`。|
|operationStatus|[groupPolicyOperationStatus](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|组策略操作状态。 可取值为：`unknown`、`inProgress`、`success`、`failed`。|
|statusDetails|String|组策略操作状态详细信息。|
|id|String|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "String",
  "operationStatus": "String",
  "statusDetails": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




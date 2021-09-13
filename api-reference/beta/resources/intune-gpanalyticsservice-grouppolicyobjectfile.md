---
title: groupPolicyObjectFile 资源类型
description: 管理员上载的组策略对象文件。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 09a3048d8b225589757463a62c7b73d5d2c8bfd1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086237"
---
# <a name="grouppolicyobjectfile-resource-type"></a>groupPolicyObjectFile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理员上载的组策略对象文件。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyObjectFiles](../api/intune-gpanalyticsservice-grouppolicyobjectfile-list.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) 集合|列出 [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) 对象的属性和关系。|
|[获取 groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-get.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|读取 [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) 对象的属性和关系。|
|[创建 groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-create.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|创建新的 [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) 对象。|
|[删除 groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-delete.md)|无|删除 [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)。|
|[更新 groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-update.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|更新 [groupPolicyObjectFile 对象](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|groupPolicyObjectId|Guid|来自 GPO Xml 内容的组策略对象 GUID|
|ouDistinguishedName|String|OU 的可分辨名称。|
|createdDateTime|DateTimeOffset|首次上载 GroupPolicy 的日期和时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改 GroupPolicyObjectFile 的日期和时间。|
|内容|String|组策略对象文件内容。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyObjectFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "id": "String (identifier)",
  "groupPolicyObjectId": "Guid",
  "ouDistinguishedName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "content": "String"
}
```




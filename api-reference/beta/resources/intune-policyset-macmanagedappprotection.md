---
title: macManagedAppProtection 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cbf530ea6b7cdc710ff54a0aed37d76a62a6389d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199969"
---
# <a name="macmanagedappprotection-resource-type"></a>macManagedAppProtection 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 macManagedAppProtections](../api/intune-policyset-macmanagedappprotection-list.md)|[macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md)集合|列出[macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md)对象的属性和关系。|
|[获取 macManagedAppProtection](../api/intune-policyset-macmanagedappprotection-get.md)|[macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md)|读取[macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md)对象的属性和关系。|
|[创建 macManagedAppProtection](../api/intune-policyset-macmanagedappprotection-create.md)|[macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md)|创建新的[macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md)对象。|
|[删除 macManagedAppProtection](../api/intune-policyset-macmanagedappprotection-delete.md)|无|删除[macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md)。|
|[更新 macManagedAppProtection](../api/intune-policyset-macmanagedappprotection-update.md)|[macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md)|更新[macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md)对象的属性。|
|[hasPayloadLinks 操作](../api/intune-policyset-macmanagedappprotection-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macManagedAppProtection",
  "id": "String (identifier)"
}
```




---
title: vulnerableManagedDevice 资源类型
description: 此实体表示与任务关联的设备。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a1f37b36b6912033dd3eb086287d5d0ab1f58cf35ed89bab97b5581e10143069
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239131"
---
# <a name="vulnerablemanageddevice-resource-type"></a>vulnerableManagedDevice 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

此实体表示与任务关联的设备。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 vulnerableManagedDevices](../api/intune-partnerintegration-vulnerablemanageddevice-list.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) 集合|列出 [vulnerableManagedDevice 对象的属性和](../resources/intune-partnerintegration-vulnerablemanageddevice.md) 关系。|
|[Get vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-get.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|读取 [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) 对象的属性和关系。|
|[创建 vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-create.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|创建新的 [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) 对象。|
|[删除 vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-delete.md)|无|删除 [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)。|
|[更新 vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-update.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|更新 [vulnerableManagedDevice 对象](../resources/intune-partnerintegration-vulnerablemanageddevice.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体密钥和 AAD 设备 ID。|
|managedDeviceId|String|Intune 托管设备 ID。|
|displayName|字符串|设备名称。|
|lastSyncDateTime|DateTimeOffset|上次同步日期。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vulnerableManagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "displayName": "String",
  "lastSyncDateTime": "String (timestamp)"
}
```





---
title: deviceLogCollectionResponse 资源类型
description: Windows 日志集合请求实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b8cde943ccfd4befad2a14f607350a9989e1e42d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299308"
---
# <a name="devicelogcollectionresponse-resource-type"></a>deviceLogCollectionResponse 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 日志集合请求实体。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 deviceLogCollectionResponses](../api/intune-devices-devicelogcollectionresponse-list.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 集合|列出 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象的属性和关系。|
|[获取 deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-get.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|读取 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象的属性和关系。|
|[创建 deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-create.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|创建新的 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象。|
|[删除 deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-delete.md)|无|删除 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)。|
|[更新 deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-update.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|更新 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象的属性。|
|[createDownloadUrl 操作](../api/intune-devices-devicelogcollectionresponse-createdownloadurl.md)|String|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|TenantId_deviceId_requestId 形式的唯一标识符|
|status|字符串|日志集合请求的状态|
|managedDeviceId|Guid|设备 Id|
|errorCode|Int64|错误代码（如果有）。 有效值-9.22337203685478 E + 18 to 9.22337203685478 E + 18|
|requestedDateTimeUTC|DateTimeOffset|请求的日期时间|
|receivedDateTimeUTC|DateTimeOffset|收到请求的日期/时间|
|initiatedByUserPrincipalName|字符串|为其启动请求的 UPN|
|expirationDateTimeUTC|DateTimeOffset|日志过期日期的日期/时间|
|大小|双精度|日志的大小。 有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceLogCollectionResponse"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
  "id": "String (identifier)",
  "status": "String",
  "managedDeviceId": "Guid",
  "errorCode": 1024,
  "requestedDateTimeUTC": "String (timestamp)",
  "receivedDateTimeUTC": "String (timestamp)",
  "initiatedByUserPrincipalName": "String",
  "expirationDateTimeUTC": "String (timestamp)",
  "size": "4.2"
}
```





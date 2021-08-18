---
title: deviceLogCollectionResponse 资源类型
description: WindowsLog Collection 请求实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fa4bffe14538618e1338b87f107148422086931e1761e171eff999eaac070626
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244734"
---
# <a name="devicelogcollectionresponse-resource-type"></a>deviceLogCollectionResponse 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

WindowsLog Collection 请求实体。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceLogCollectionResponses](../api/intune-devices-devicelogcollectionresponse-list.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 集合|列出 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象的属性和关系。|
|[获取 deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-get.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|读取 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象的属性和关系。|
|[创建 deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-create.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|创建新的 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象。|
|[删除 deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-delete.md)|无|删除 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)。|
|[更新 deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-update.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|更新 [deviceLogCollectionResponse 对象](../resources/intune-devices-devicelogcollectionresponse.md) 的属性。|
|[createDownloadUrl 操作](../api/intune-devices-devicelogcollectionresponse-createdownloadurl.md)|String|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|表单的唯一标识符tenantId_deviceId_requestId|
|status|字符串|日志集合请求的状态|
|managedDeviceId|Guid|设备 ID|
|errorCode|Int64|错误代码（如果有）。 有效值 -9.22337203685478E+18 到 9.22337203685478E+18|
|requestedDateTimeUTC|DateTimeOffset|请求的 DateTime|
|receivedDateTimeUTC|DateTimeOffset|收到请求的日期/时间|
|initiatedByUserPrincipalName|字符串|发起请求的 UPN|
|expirationDateTimeUTC|DateTimeOffset|日志过期的 DateTime|
|size|双精度|日志的大小。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|

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





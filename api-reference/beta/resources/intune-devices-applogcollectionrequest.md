---
title: appLogCollectionRequest 资源类型
description: AppLogCollectionRequest 实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 795b80b0194f2c3a1d314cbb317af954fb675063
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431348"
---
# <a name="applogcollectionrequest-resource-type"></a>appLogCollectionRequest 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLogCollectionRequest 实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 appLogCollectionRequests](../api/intune-devices-applogcollectionrequest-list.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)集合|列出属性和[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象之间的关系。|
|[获取 appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|读取属性和[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象的关系。|
|[创建 appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-create.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|创建新的[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象。|
|[删除 appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-delete.md)|无|删除[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)。|
|[更新 appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-update.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|更新[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象的属性。|
|[createDownloadUrl 操作](../api/intune-devices-applogcollectionrequest-createdownloadurl.md)|[appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md)|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|唯一的标识符。 这是 userId_DeviceId_AppId id。|
|status|[appLogUploadState](../resources/intune-devices-apploguploadstate.md)|日志上载状态。 可取值为：`pending`、`completed`、`failed`。|
|errorMessage|String|如果在上载过程中的任何错误消息|
|customLogFolders|String 集合|日志文件文件夹的列表。 |
|completedDateTime|DateTimeOffset|上载日志请求频率达到终端状态的时间|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "String (identifier)",
  "status": "String",
  "errorMessage": "String",
  "customLogFolders": [
    "String"
  ],
  "completedDateTime": "String (timestamp)"
}
```





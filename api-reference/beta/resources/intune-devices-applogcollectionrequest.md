---
title: appLogCollectionRequest 资源类型
description: AppLogCollectionRequest 实体。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e2cd37ecd109720bf5a564c64d480037a9bd72fc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086307"
---
# <a name="applogcollectionrequest-resource-type"></a>appLogCollectionRequest 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLogCollectionRequest 实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 appLogCollectionRequests](../api/intune-devices-applogcollectionrequest-list.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) 集合|列出 [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) 对象的属性和关系。|
|[获取 appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|读取 [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) 对象的属性和关系。|
|[创建 appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-create.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|创建新的 [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) 对象。|
|[删除 appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-delete.md)|无|删除 [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)。|
|[更新 appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-update.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|更新 [appLogCollectionRequest 对象](../resources/intune-devices-applogcollectionrequest.md) 的属性。|
|[createDownloadUrl 操作](../api/intune-devices-applogcollectionrequest-createdownloadurl.md)|[appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md)|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|唯一标识符。 这是userId_DeviceId_AppId ID。|
|status|[appLogUploadState](../resources/intune-devices-apploguploadstate.md)|记录上载状态。 可取值为：`pending`、`completed`、`failed`。|
|errorMessage|String|上传过程中出现错误消息（如果有）|
|customLogFolders|字符串集合|日志文件夹列表。 |
|completedDateTime|DateTimeOffset|上载日志请求达到终端状态的时间|

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




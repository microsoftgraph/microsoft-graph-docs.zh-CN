---
title: teamworkDeviceOperation 资源类型
description: 表示有关在启用了 Microsoft Teams 设备上运行的异步操作的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 513e18da8ed8432ce988c15f9737944d2493df3d
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262423"
---
# <a name="teamworkdeviceoperation-resource-type"></a>teamworkDeviceOperation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关在启用了[Microsoft Teams设备上运行的](../resources/teamworkdevice.md)异步操作的详细信息，包括操作状态。 在设备上运行的任何异步操作将创建 **一个 teamworkDeviceOperation** 对象。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 teamworkDeviceOperations](../api/teamworkdeviceoperation-list.md)|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md) 集合|获取 [teamworkDeviceOperation 对象](../resources/teamworkdeviceoperation.md) 及其属性的列表。|
|[获取 teamworkDeviceOperation](../api/teamworkdeviceoperation-get.md)|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|读取 [teamworkDeviceOperation](../resources/teamworkdeviceoperation.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|completedDateTime|DateTimeOffset|操作达到最终状态的时间 (例如、 `Successful``Failed``Cancelled` 和) 。|
|createdBy|[identitySet](../resources/identityset.md)|创建设备操作的用户的标识。|
|createdDateTime|DateTimeOffset|创建设备操作时 UTC 日期和时间。|
|error|[operationError](../resources/operationerror.md)|错误详细信息仅在状态失败时可用。|
|id|String|文档标识符。 继承自 [实体](../resources/entity.md)。|
|lastActionBy|[identitySet](../resources/identityset.md)|上次修改设备操作的用户的标识。|
|lastActionDateTime|DateTimeOffset|设备操作上次修改的 UTC 日期和时间。|
|operationType|teamworkDeviceOperationType|设备上异步操作的类型。 可能的值是：、`deviceRestart`、`configUpdate`、`deviceDiagnostics`、`softwareUpdate`、`deviceManagementAgentConfigUpdate`、`remoteLogin`、`remoteLogout``unknownFutureValue`。|
|startedDateTime|DateTimeOffset|启动操作的时间。|
|状态|String|异步操作的当前状态，`Queued``Scheduled``Successful``InProgress``Cancelled`例如、 和 。`Failed`|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDeviceOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceOperation",
  "completedDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.operationError"
  },
  "id": "String (identifier)",
  "lastActionBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastActionDateTime": "String (timestamp)",
  "operationType": "String",
  "startedDateTime": "String (timestamp)",
  "status": "String"
}
```


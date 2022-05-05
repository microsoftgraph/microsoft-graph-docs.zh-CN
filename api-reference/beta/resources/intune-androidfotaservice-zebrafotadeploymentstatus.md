---
title: zebraFotaDeploymentStatus 资源类型
description: 描述单个 FOTA 部署的状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bcc9c905c580b8d20d1bd43ed818e339aaa7ff93
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213181"
---
# <a name="zebrafotadeploymentstatus-resource-type"></a>zebraFotaDeploymentStatus 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述单个 FOTA 部署的状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|state|[zebraFotaDeploymentState](../resources/intune-androidfotaservice-zebrafotadeploymentstate.md)|有关可能的值，请参阅 zebraFotaDeploymentState 枚举。 可取值为：`pendingCreation`、`createFailed`、`created`、`inProgress`、`completed`、`pendingCancel`、`canceled`、`unknownFutureValue`。|
|totalDevices|Int32|一个整数，指示部署中的设备总数。|
|totalCreated|Int32|一个整数，指示处于 CREATED 状态的作业的设备总数。 通常指示未到达设备的作业。 |
|totalScheduled|Int32|一个整数，指示接收 json 并已计划的设备总数。 |
|totalDownloading|Int32|一个整数，指示成功安装的设备总数。|
|totalAwaitingInstall|Int32|一个整数，指示成功安装的设备总数。|
|totalSucceededInstall|Int32|一个整数，指示成功安装的设备总数。|
|totalCanceled|Int32|一个整数，指示已取消安装的设备总数。|
|totalUnknown|Int32|一个整数，指示未收到部署状态或结束状态的设备总数，即使在达到计划的结束日期之后。|
|totalFailedDownload|Int32|一个整数，指示未能下载新 OS 文件的设备总数。|
|totalFailedInstall|Int32|一个整数，指示未能安装新 OS 文件的设备总数。|
|completeOrCanceledDateTime|DateTimeOffset|完成或取消此部署的日期和时间。 实际日期时间由状态值决定。 如果状态已取消，此属性将保留取消日期/时间。 如果状态已完成，则此属性保留完成日期/时间。 如果部署未在部署结束日期之前完成，则完成的日期/时间和结束日期/时间相同。 这始终位于部署时区中。 注意：正在进行的安装可以继续超过部署结束日期。|
|cancelRequested|Boolean|一个布尔值，指示是否在部署中请求取消。 注意：取消请求不保证部署已取消。|
|lastUpdatedDateTime|DateTimeOffset| 从 Zebra 更新部署状态的日期和时间|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.zebraFotaDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaDeploymentStatus",
  "state": "String",
  "totalDevices": 1024,
  "totalCreated": 1024,
  "totalScheduled": 1024,
  "totalDownloading": 1024,
  "totalAwaitingInstall": 1024,
  "totalSucceededInstall": 1024,
  "totalCanceled": 1024,
  "totalUnknown": 1024,
  "totalFailedDownload": 1024,
  "totalFailedInstall": 1024,
  "completeOrCanceledDateTime": "String (timestamp)",
  "cancelRequested": true,
  "lastUpdatedDateTime": "String (timestamp)"
}
```





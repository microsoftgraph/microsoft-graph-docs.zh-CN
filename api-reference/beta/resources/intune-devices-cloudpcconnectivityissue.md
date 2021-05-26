---
title: cloudPCConnectivityIssue 资源类型
description: 用户体验分析连接问题实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7e54a76735b765c43aadd248095f26fad692427d
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666851"
---
# <a name="cloudpcconnectivityissue-resource-type"></a>cloudPCConnectivityIssue 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析连接问题实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 cloudPCConnectivityIssues](../api/intune-devices-cloudpcconnectivityissue-list.md)|[cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) 集合|列出 [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) 对象的属性和关系。|
|[获取 cloudPCConnectivityIssue](../api/intune-devices-cloudpcconnectivityissue-get.md)|[cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md)|读取 [cloudPCConnectivityIssue 对象的属性和](../resources/intune-devices-cloudpcconnectivityissue.md) 关系。|
|[创建 cloudPCConnectivityIssue](../api/intune-devices-cloudpcconnectivityissue-create.md)|[cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md)|创建新的 [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) 对象。|
|[删除 cloudPCConnectivityIssue](../api/intune-devices-cloudpcconnectivityissue-delete.md)|无|删除 [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md)。|
|[更新 cloudPCConnectivityIssue](../api/intune-devices-cloudpcconnectivityissue-update.md)|[cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md)|更新 [cloudPCConnectivityIssue 对象](../resources/intune-devices-cloudpcconnectivityissue.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析连接问题事件实体的唯一标识符。|
|deviceId|String|与连接关联的设备的 Intune DeviceId。|
|errorCode|String|连接问题的错误代码。|
|errorDateTime|DateTimeOffset|连接启动的时间。 时间以 ISO 8601 格式显示，协调世界时 (UTC) 时间。|
|userId|String|初始化连接的用户的唯一 ID。|
|errorDescription|String|错误的详细说明。|
|recommendedAction|String|修复相应错误的推荐操作。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPCConnectivityIssue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "id": "String (identifier)",
  "deviceId": "String",
  "errorCode": "String",
  "errorDateTime": "String (timestamp)",
  "userId": "String",
  "errorDescription": "String",
  "recommendedAction": "String"
}
```





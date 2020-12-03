---
title: cloudPC 资源类型
description: 云托管虚拟桌面。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d1109ceb81f741cefa9b26662bc1c8c5de8a8329
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563826"
---
# <a name="cloudpc-resource-type"></a>cloudPC 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云管理的虚拟桌面。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[cloudPC](../resources/cloudpc.md) 集合|列出 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。|
|[获取 cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|读取 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。|
|[重新设置](../api/cloudpc-reprovision.md)|无|重新设置一个 [cloudPC](../resources/cloudpc.md) 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|云电脑的唯一标识符。 只读。|
|displayName|String|云电脑显示名称。|
|imageDisplayName|String|云电脑上的 OS 映像的名称。|
|managedDeviceId|String|云电脑的 Intune 设备 ID。|
|managedDeviceName|String|云电脑的 Intune 设备名称。|
|provisioningPolicyId|String|云电脑的设置策略 ID。|
|servicePlanId|String|云电脑的服务计划 ID。|
|servicePlanName|String|云电脑的服务计划名称。|
|status|cloudPcStatus|云电脑的状态。 可取值为：`notProvisioned`、`provisioning`、`provisioned`、`upgrading`、`inGracePeriod`、`deprovisioning`、`upgradeFailed`、`provisionFailed`、`deprovisionFailed`、`reprovisionFailed`。|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|云电脑状态的详细信息。|
|userPrincipalName|String|为云电脑分配的用户的用户主体名称 (UPN) 。|
|lastModifiedDateTime|DateTimeOffset|云电脑的上次修改日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPC",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPC",
  "id": "String (identifier)",
  "displayName": "String",
  "imageDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "provisioningPolicyId": "String",
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

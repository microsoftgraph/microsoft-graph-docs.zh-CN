---
title: cloudPC 资源类型
description: 云托管虚拟桌面。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 95758299f87ac463bac6fdc30f7d70fb59eb6c92
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378317"
---
# <a name="cloudpc-resource-type"></a>cloudPC 资源类型

命名空间：microsoft.graph

表示云管理的虚拟桌面。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[cloudPC](../resources/cloudpc.md) 集合|列出 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。|
|[获取 cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|读取 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。|
|[重新设置](../api/cloudpc-reprovision.md)|无|重新设置一个 [cloudPC](../resources/cloudpc.md) 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|云电脑的唯一标识符。 只读。|
|displayName|字符串|云电脑显示名称。|
|imageDisplayName|字符串|云电脑上的 OS 映像的名称。|
|managedDeviceId|字符串|云电脑的 Intune 设备 ID。|
|managedDeviceName|String|云电脑的 Intune 设备名称。|
|provisioningPolicyId|字符串|云电脑的设置策略 ID。|
|servicePlanId|字符串|云电脑的服务计划 ID。|
|servicePlanName|String|云电脑的服务计划名称。|
|status|cloudPcStatus|云电脑的状态。 可取值为：`notProvisioned`、`provisioning`、`provisioned`、`upgrading`、`inGracePeriod`、`deprovisioning`、`upgradeFailed`、`provisionFailed`、`deprovisionFailed`、`reprovisionFailed`。|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|云电脑状态的详细信息。|
|userPrincipalName|字符串|为云电脑分配的用户的用户主体名称 (UPN) 。|
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

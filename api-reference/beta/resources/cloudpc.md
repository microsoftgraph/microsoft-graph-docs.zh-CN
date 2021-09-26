---
title: cloudPC 资源类型
description: 云托管虚拟桌面。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: e3f716b059a55f12add0eaf0b8ab785f71e1cb42
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765198"
---
# <a name="cloudpc-resource-type"></a>cloudPC 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云托管虚拟桌面。 此云电脑还注册到 Intune 中，并通过 MEM 门户进行管理，因此云电脑还具有相应的 Intune 托管设备 ID。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[cloudPC](../resources/cloudpc.md) 集合|列出 [cloudPC 对象的属性和](../resources/cloudpc.md) 关系。|
|[获取 cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|读取 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。|
|[重新设置](../api/cloudpc-reprovision.md)|无|重新设置 [cloudPC](../resources/cloudpc.md) 对象。|
|[endGracePeriod](../api/cloudpc-endgraceperiod.md)|无|结束 [cloudPC](../resources/cloudpc.md) 对象的宽限期。|
|[重新设置 cloudPC 远程操作](../api/manageddevice-reprovisioncloudpc.md)|无|使用 Intune 托管的设备 ID 重新设置云电脑。|
|[批量重新设置 cloudPCs 远程操作](../api/manageddevice-bulkreprovisioncloudpc.md)|无|使用 Intune 托管的设备 ID 批量重新预配一组云电脑设备。|
|[调整 cloudPC 远程操作的大小](../api/manageddevice-resizecloudpc.md)|无|通过 Intune 托管设备 ID 将现有 CloudPC 升级或降级为具有新 vCPU 和存储大小的另一个配置。|
|[获取 cloudPC 远程操作结果](../api/manageddevice-getcloudpcremoteactionresults.md)|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|检查 [云电脑设备的云](../resources/cloudpcremoteactionresult.md) 电脑指定的远程操作结果。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|云电脑的唯一标识符。 只读。|
|displayName|String|云电脑显示名称。|
|imageDisplayName|String|云电脑上的操作系统映像的名称。|
|managedDeviceId|String|云电脑的 Intune 设备 ID。|
|managedDeviceName|String|云电脑的 Intune 设备名称。|
|provisioningPolicyId|String|云电脑的预配策略 ID。|
|provisioningPolicyName|String|预配云电脑期间应用的预配策略。|
|onPremisesConnectionName|String|预配云电脑期间应用本地连接。|
|servicePlanId|String|云电脑的服务计划 ID。|
|servicePlanName|String|云电脑的服务计划名称。|
|status|[cloudPcStatus](#cloudpcstatus-values)|云电脑的状态。 可取值为：`notProvisioned`、`provisioning`、`provisioned`、`upgrading`、`inGracePeriod`、`deprovisioning` 或 `failed`。|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|云电脑状态的详细信息。|
|userPrincipalName|String|用户主体名称 (分配给) 电脑的用户的 UPN 名称。|
|lastModifiedDateTime|DateTimeOffset|云电脑上次修改的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|gracePeriodEndDateTime|DateTimeOffset|宽限期结束和重新设置/取消设置发生的日期和时间。 仅在 status 为 时是必需的 `inGracePeriod` 。 时间戳以 ISO 8601 格式和 UTC 协调世界时 (显示) 。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|

### <a name="cloudpcstatus-values"></a>cloudPcStatus 值

|成员|说明|
|:---|:---|
|notProvisioned|尚未预配云电脑。|
|预配|云电脑预配正在进行中。|
|已设置|云电脑已预配，最终用户可以访问它。|
|inGracePeriod|云电脑在取消预配前的一周内宽限期内。|
|取消设置|云电脑正在取消设置。|
|failed|云电脑上的操作已失败。|
|provisionedWithWarnings|云电脑已预配，最终用户可以访问它，但有一些警告。 用户可以继续使用此云电脑。|
|调整大小|云电脑正在调整大小。|
|unknownFutureValue|可发展枚举 sentinel 值。 请勿使用。|

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
  "provisioningPolicyName": "String",
  "onPremisesConnectionName": "String",
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "gracePeriodEndDateTime": "String (timestamp)"
}
```

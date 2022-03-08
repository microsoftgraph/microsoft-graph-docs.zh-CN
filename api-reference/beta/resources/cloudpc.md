---
title: cloudPC 资源类型
description: 云托管虚拟桌面。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 9edd626ae9914941a18801791e942c1dfd69e391
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336912"
---
# <a name="cloudpc-resource-type"></a>cloudPC 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云托管虚拟桌面。 此云电脑还注册到 Intune 中，并通过 Microsoft Endpoint Manager 门户进行管理，因此云电脑还具有相应的 Intune 托管设备 ID。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[cloudPC](../resources/cloudpc.md) 集合|列出 [cloudPC 对象的属性和](../resources/cloudpc.md) 关系。|
|[获取 cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|读取 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。|
|[更改用户帐户类型](../api/cloudpc-changeuseraccounttype.md)|无|更改特定云电脑上用户的帐户类型。|
|[结束宽限期](../api/cloudpc-endgraceperiod.md)|无|结束 [cloudPC 对象的宽限期](../resources/cloudpc.md) 。|
|[获取远程操作结果](../api/manageddevice-getcloudpcremoteactionresults.md)|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|检查 [云电脑设备的云](../resources/cloudpcremoteactionresult.md) 电脑指定的远程操作结果。|
|[重新启动](../api/cloudpc-reboot.md)|无|重新启动特定的 [cloudPC](../resources/cloudpc.md) 对象。|
|[Rename](../api/cloudpc-rename.md)|无|重命名特定的 [cloudPC](../resources/cloudpc.md) 对象。 使用此 API 更新 **云电脑实体的 displayName** 。|
|[重新设置](../api/cloudpc-reprovision.md)|无|重新设置 [cloudPC](../resources/cloudpc.md) 对象。|
|[重新设置远程操作](../api/manageddevice-reprovisioncloudpc.md)|无|使用  [Intune 托管](../resources/cloudpc.md) 的设备 ID 重新设置云电脑。|
|[批量重新设置远程操作](../api/manageddevice-bulkreprovisioncloudpc.md)|无|使用 Intune 托管的设备 ID 批量重新预配一组云电脑设备。|
|[调整远程操作大小](../api/manageddevice-resizecloudpc.md)|无|通过 Intune 托管设备 ID 将现有云电脑升级或降级为具有新 vCPU 和存储大小的另一配置。|
|[疑难解答](../api/cloudpc-troubleshoot.md)|无|特定 [cloudPC 对象疑](../resources/cloudpc.md) 难解答。 使用此 API 检查云电脑和会话主机的运行状况。|
|[还原远程操作](../api/manageddevice-restorecloudpc.md)|无|将云电脑设备从快照还原到以前的状态。|
|[批量还原远程操作](../api/manageddevice-bulkrestorecloudpc.md)|[cloudPcBulkRemoteActionResult](../resources/cloudpcbulkremoteactionresult.md)|使用单个请求还原多个云电脑设备，其中包括 Intune 托管设备的 ID 和还原点日期和时间。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|aadDeviceId|字符串|云Azure Active Directory (Azure AD) 的设备 ID。|
|displayName|String|云显示名称的屏幕。|
|gracePeriodEndDateTime|DateTimeOffset|宽限期结束和重新设置/取消设置发生的日期和时间。 仅在状态为 时是必需的 `inGracePeriod`。 时间戳以 ISO 8601 格式和 UTC 协调世界时 (显示) 。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|id|String|云电脑的唯一标识符。 只读。|
|imageDisplayName|字符串|云电脑上的操作系统映像的名称。|
|lastLoginResult|[cloudPcLoginResult](../resources/cloudpcloginresult.md)|云电脑的最后登录结果。 例如，`{ "time": "2014-01-01T00:00:00Z"}`。|
|lastModifiedDateTime|DateTimeOffset|云电脑上次修改的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|lastRemoteActionResult|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|企业云电脑的最后远程操作结果。 支持的远程操作包括：、`Reboot`、`Rename``Reprovision`、`Restore`和 `Troubleshoot`。|
|managedDeviceId|String|云电脑的 Intune 设备 ID。|
|managedDeviceName|String|云电脑的 Intune 设备名称。|
|onPremisesConnectionName|String|预配云电脑期间应用本地连接。|
|osVersion|[cloudPcOperatingSystem](../resources/cloudpcorganizationsettings.md#cloudpcoperatingsystem-values)|操作系统版本 (操作系统) 在云 PC 上预配。 可能的值是：、`windows10``windows11`和 `unknownFutureValue`。|
|provisioningPolicyId|String|云电脑的预配策略 ID。|
|provisioningPolicyName|String|预配云电脑期间应用的预配策略。|
|servicePlanId|String|云电脑的服务计划 ID。|
|servicePlanName|String|云电脑的服务计划名称。|
|servicePlanType|[cloudPcServicePlanType](../resources/cloudpcserviceplan.md#cloudpcserviceplantype-values)|云电脑的服务计划类型。|
|状态|[cloudPcStatus](#cloudpcstatus-values)|云电脑的状态。 可取值为：`notProvisioned`、`provisioning`、`provisioned`、`upgrading`、`inGracePeriod`、`deprovisioning`、`failed`、`restoring`。|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|云电脑状态的详细信息。|
|userAccountType|[cloudPcUserAccountType](../resources/cloudpcorganizationsettings.md#cloudpcuseraccounttype-values)|已预配云 PC 上的用户的帐户类型。 可能的值是：、`standardUser``administrator`和 `unknownFutureValue`。|
|userPrincipalName|String|用户主体名称 (分配给) 电脑的用户的 UPN 名称。|

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
|pendingProvision|预配在云电脑上挂起。 在这种情况下，宽限期内云电脑的数量大于可用许可证总数。 |
|还原|正在还原云电脑。|
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
  "aadDeviceId": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "provisioningPolicyId": "String",
  "provisioningPolicyName": "String",
  "onPremisesConnectionName": "String",
  "servicePlanId": "String",
  "servicePlanType": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "gracePeriodEndDateTime": "String (timestamp)",
  "userAccountType": "String",
  "osVersion": "String",
  "lastRemoteActionResult": "String",
  "lastLoginResult": "String"
}
```

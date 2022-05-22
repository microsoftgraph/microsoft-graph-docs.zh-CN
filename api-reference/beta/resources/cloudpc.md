---
title: cloudPC 资源类型
description: 云托管虚拟桌面。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: f529b46fc5bb11be7f58fbd4068789d5def4e824
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628850"
---
# <a name="cloudpc-resource-type"></a>cloudPC 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云托管的虚拟桌面。 此云电脑也已注册到Intune并通过Microsoft Endpoint Manager门户进行管理，因此云电脑还具有相应的Intune托管设备 ID。

## <a name="methods"></a>方法

|方法|返回类型|Description|
|:---|:---|:---|
|[列出 cloudPC](../api/virtualendpoint-list-cloudpcs.md)|[cloudPC](../resources/cloudpc.md) 集合|列出 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。|
|[获取 cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|读取 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。|
|[更改用户帐户类型](../api/cloudpc-changeuseraccounttype.md)|无|更改特定云电脑上用户的帐户类型。|
|[结束宽限期](../api/cloudpc-endgraceperiod.md)|无|结束 [cloudPC](../resources/cloudpc.md) 对象的宽限期。|
|[获取远程操作结果](../api/manageddevice-getcloudpcremoteactionresults.md)|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|检查 [云电脑设备的云电脑指定的远程操作结果](../resources/cloudpcremoteactionresult.md) 。|
|[重新 启动](../api/cloudpc-reboot.md)|无|重新启动特定 [的 cloudPC](../resources/cloudpc.md) 对象。|
|[Rename](../api/cloudpc-rename.md)|无|重命名特定 [的 cloudPC](../resources/cloudpc.md) 对象。 使用此 API 更新 Cloud PC 实体的 **displayName** 。|
|[重新预配](../api/cloudpc-reprovision.md)|无|重新预配 [cloudPC](../resources/cloudpc.md) 对象。|
|[重新预配远程操作](../api/manageddevice-reprovisioncloudpc.md)|无|使用Intune[管理的设备](../resources/cloudpc.md) ID 重新预配云电脑。  |
|[批量重新预配远程操作](../api/manageddevice-bulkreprovisioncloudpc.md)|无|使用Intune托管设备 ID 批量重新预配一组云电脑设备。|
|[调整远程操作的大小](../api/manageddevice-resizecloudpc.md)|无|通过Intune托管设备 ID 将现有云电脑升级或降级到具有新 vCPU 和存储大小的另一个配置。|
|[疑难解答](../api/cloudpc-troubleshoot.md)|无|对特定 [cloudPC](../resources/cloudpc.md) 对象进行故障排除。 使用此 API 检查云电脑和会话主机的运行状况。|
|[还原远程操作](../api/manageddevice-restorecloudpc.md)|无|从快照将云电脑设备还原到以前的状态。|
|[批量还原远程操作](../api/manageddevice-bulkrestorecloudpc.md)|[cloudPcBulkRemoteActionResult](../resources/cloudpcbulkremoteactionresult.md)|使用单个请求还原多个云电脑设备，其中包括Intune托管设备的 ID 以及还原点日期和时间。|
|[设置审阅状态](../api/manageddevice-setcloudpcreviewstatus.md)|无|设置特定云电脑设备的审阅状态。|
|[获取审阅状态](../api/manageddevice-getcloudpcreviewstatus.md)|[cloudPcReviewStatus](../resources/cloudpcreviewstatus.md)|获取特定云电脑设备的审阅状态。|
|[批量集审阅状态](../api/manageddevice-bulksetcloudpcreviewstatus.md)|[cloudPcBulkRemoteActionResult](../resources/cloudpcbulkremoteactionresult.md)|使用包含Intune托管设备 ID 的单个请求设置多个云电脑设备的审阅状态。|
|[用户列表](../api/user-list-cloudpcs.md)|[cloudPC](../resources/cloudpc.md) 集合|列出归属于已登录用户的 [cloudPC](../resources/cloudpc.md) 设备。|
|[获取用户的启动信息](../api/cloudpc-getcloudpclaunchinfo.md)|[cloudPCLaunchInfo](../resources/cloudpclaunchinfo.md)|获取已登录用户的 [cloudPCLaunchInfo](../resources/cloudpclaunchinfo.md) 。|

## <a name="properties"></a>属性

|属性|类型|Description|
|:---|:---|:---|
|aadDeviceId|字符串|Azure Active Directory (Azure AD) 云电脑的设备 ID。|
|displayName|字符串|云电脑的显示名称。|
|gracePeriodEndDateTime|DateTimeOffset|宽限期结束和重新预配/取消预配的日期和时间。 仅当状态为 `inGracePeriod`.. 时间戳以 ISO 8601 格式显示，协调世界时 (UTC) 。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|id|String|云电脑的唯一标识符。 只读。|
|imageDisplayName|字符串|云电脑上的 OS 映像的名称。|
|lastLoginResult|[cloudPcLoginResult](../resources/cloudpcloginresult.md)|云电脑的最后一次登录结果。 例如，`{ "time": "2014-01-01T00:00:00Z"}`。|
|lastModifiedDateTime|DateTimeOffset|云电脑的上次修改日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|lastRemoteActionResult|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|企业云电脑的最后一个远程操作结果。 支持的远程操作包括：`Reboot`、`Rename`、`Reprovision`和 `Restore``Troubleshoot`。|
|managedDeviceId|String|云电脑的Intune设备 ID。|
|managedDeviceName|String|云电脑的Intune设备名称。|
|onPremisesConnectionName|字符串|在预配云电脑期间应用的 Azure 网络连接。|
|osVersion|[cloudPcOperatingSystem](../resources/cloudpcorganizationsettings.md#cloudpcoperatingsystem-values)|操作系统版本 (操作系统) 在云电脑上进行预配。 可能的值为： `windows10`和 `windows11``unknownFutureValue`.|
|provisioningPolicyId|String|云电脑的预配策略 ID。|
|provisioningPolicyName|字符串|在预配云电脑期间应用的预配策略。|
|servicePlanId|String|云电脑的服务计划 ID。|
|servicePlanName|String|云电脑的服务计划名称。|
|servicePlanType|[cloudPcServicePlanType](../resources/cloudpcserviceplan.md#cloudpcserviceplantype-values)|云电脑的服务计划类型。|
|status|[cloudPcStatus](#cloudpcstatus-values)|云电脑的状态。 可取值为：`notProvisioned`、`provisioning`、`provisioned`、`upgrading`、`inGracePeriod`、`deprovisioning`、`failed`、`restoring`。|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|云电脑状态的详细信息。|
|userAccountType|[cloudPcUserAccountType](../resources/cloudpcorganizationsettings.md#cloudpcuseraccounttype-values)|预配的云电脑上用户的帐户类型。 可能的值为： `standardUser`和 `administrator``unknownFutureValue`.|
|userPrincipalName|字符串|分配给云电脑的用户的用户主体名称 (UPN) 。|

### <a name="cloudpcstatus-values"></a>cloudPcStatus 值

|成员|说明|
|:---|:---|
|notProvisioned|尚未预配云电脑。|
|供应|云电脑预配正在进行中。|
|已设置|云电脑已预配，可由最终用户访问。|
|inGracePeriod|云电脑在取消预配之前的一周宽限期内。|
|取消预配|云电脑正在取消预配。|
|失败|云电脑上的操作已失败。|
|provisionedWithWarnings|云电脑已预配，可由最终用户访问，但会出现一些警告。 用户可以继续使用此云电脑。|
|调整|云电脑正在调整大小。|
|pendingProvision|云电脑上正在等待预配。 在这种情况下，宽限期内云电脑的数量大于可用许可证总数。 |
|恢复|云电脑正在还原。|
|unknownFutureValue|可变枚举 sentinel 值。 请勿使用。|

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

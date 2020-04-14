---
title: androidForWorkSettings 资源类型
description: Android for Work 设置。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 50153f0db801764aa22872468b87f5c7eaf1cbaf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459198"
---
# <a name="androidforworksettings-resource-type"></a>androidForWorkSettings 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android for Work 设置。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 androidForWorkSettings](../api/intune-androidforwork-androidforworksettings-get.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|读取 [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) 对象的属性和关系。|
|[更新 androidForWorkSettings](../api/intune-androidforwork-androidforworksettings-update.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|更新 [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) 对象的属性。|
|[requestSignupUrl 操作](../api/intune-androidforwork-androidforworksettings-requestsignupurl.md)|String|尚未记录|
|[completeSignup 操作](../api/intune-androidforwork-androidforworksettings-completesignup.md)|无|尚未记录|
|[syncApps 操作](../api/intune-androidforwork-androidforworksettings-syncapps.md)|无|尚未记录|
|[取消绑定操作](../api/intune-androidforwork-androidforworksettings-unbind.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Android for Work 设置标识符|
|bindStatus|[androidForWorkBindStatus](../resources/intune-androidforwork-androidforworkbindstatus.md)|使用 Google EMM API 的租户的绑定状态。 可取值为：`notBound`、`bound`、`boundAndValidated`、`unbinding`。|
|lastAppSyncDateTime|DateTimeOffset|应用同步的上次完成时间|
|lastAppSyncStatus|[androidForWorkSyncStatus](../resources/intune-androidforwork-androidforworksyncstatus.md)|上次应用程序同步结果。 可取值为：`success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。|
|ownerUserPrincipalName|String|创建了企业的所有者 UPN|
|ownerOrganizationName|String|载入 Android for Work 时使用的组织名称|
|lastModifiedDateTime|DateTimeOffset|Android for Work 设置的上次修改时间|
|enrollmentTarget|[androidForWorkEnrollmentTarget](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|指示哪些用户可以在 Android for Work 设备管理中注册设备。 可取值为：`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions`。|
|targetGroupIds|String collection|指定当 enrollmentTarget 设置为“定向”时可以在 Android for Work 设备管理中注册设备的 AAD 组。|
|deviceOwnerManagementEnabled|布尔值|指示此帐户是否为使用 CloudDPC 的 Android 设备所有者管理 flighting。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ],
  "deviceOwnerManagementEnabled": true
}
```




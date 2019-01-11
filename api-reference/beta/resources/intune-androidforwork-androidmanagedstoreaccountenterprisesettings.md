---
title: androidManagedStoreAccountEnterpriseSettings 资源类型
description: Android 的企业设置管理存储的帐户。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: db31210da358a8b6b7ebc674699dab4c622ae670
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869032"
---
# <a name="androidmanagedstoreaccountenterprisesettings-resource-type"></a>androidManagedStoreAccountEnterpriseSettings 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Android 的企业设置管理存储的帐户。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 androidManagedStoreAccountEnterpriseSettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|读取属性和[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)对象的关系。|
|[更新 androidManagedStoreAccountEnterpriseSettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-update.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|更新[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)对象的属性。|
|[requestSignupUrl 操作](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl.md)|String|尚未记录|
|[completeSignup 操作](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup.md)|无|尚未记录|
|[syncApps 操作](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps.md)|无|尚未记录|
|[取消绑定操作](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind.md)|无|尚未记录|
|[createGooglePlayWebToken 操作](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken.md)|字符串|生成嵌入组件中使用的 web 标记。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|Android 存储帐户企业设置标识符|
|bindStatus|[androidManagedStoreAccountBindStatus](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|将绑定使用 Google EMM API 的租户的状态。 可取值为：`notBound`、`bound`、`boundAndValidated`、`unbinding`。|
|lastAppSyncDateTime|DateTimeOffset|应用同步的上次完成时间|
|lastAppSyncStatus|[androidManagedStoreAccountAppSyncStatus](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|最后一个应用程序同步结果。 可取值为：`success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。|
|ownerUserPrincipalName|String|创建了企业的所有者 UPN|
|ownerOrganizationName|String|何时使用组织名称入职培训 Android 企业|
|lastModifiedDateTime|DateTimeOffset|上次修改时间 Android 企业设置|
|enrollmentTarget|[androidManagedStoreAccountEnrollmentTarget](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|指示哪些用户可以注册 Android 企业设备管理的设备。 可取值为：`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions`。|
|targetGroupIds|String 集合|指定当 enrollmentTarget 设置为“定向”时可以在 Android for Work 设备管理中注册设备的 AAD 组。|
|deviceOwnerManagementEnabled|布尔|指示是否此帐户 flighting 用于与 CloudDPC Android 设备所有者管理。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAccountEnterpriseSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
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






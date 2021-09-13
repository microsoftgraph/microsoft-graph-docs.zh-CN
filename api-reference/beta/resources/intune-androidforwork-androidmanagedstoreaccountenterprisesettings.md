---
title: androidManagedStoreAccountEnterpriseSettings 资源类型
description: Enterprise Android 托管存储帐户的设置。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f06f7d042977605214a286ec76ec4fd9c5ee88ca
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101910"
---
# <a name="androidmanagedstoreaccountenterprisesettings-resource-type"></a>androidManagedStoreAccountEnterpriseSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Enterprise Android 托管存储帐户的设置。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 androidManagedStoreAccountEnterpriseSettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|读取 [androidManagedStoreAccountEnterpriseSettings 对象的属性和](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) 关系。|
|[更新 androidManagedStoreAccountEnterpriseSettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-update.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|更新 [androidManagedStoreAccountEnterpriseSettings 对象](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) 的属性。|
|[approveApps 操作](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-approveapps.md)|无|尚未记录|
|[requestSignupUrl 操作](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl.md)|String|尚未记录|
|[completeSignup 操作](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup.md)|无|尚未记录|
|[syncApps 操作](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps.md)|无|尚未记录|
|[取消绑定操作](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind.md)|无|尚未记录|
|[createGooglePlayWebToken 操作](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken.md)|String|生成在可嵌入组件中使用的 Web 令牌。|
|[setAndroidDeviceOwnerFullyManagedEnrollmentState 操作](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-setandroiddeviceownerfullymanagedenrollmentstate.md)|无|将 AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled 设置为给定值。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Android 应用商店帐户企业设置标识符|
|bindStatus|[androidManagedStoreAccountBindStatus](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|使用 Google EMM API 绑定租户的状态。 可取值为：`notBound`、`bound`、`boundAndValidated`、`unbinding`。|
|lastAppSyncDateTime|DateTimeOffset|应用同步的上次完成时间|
|lastAppSyncStatus|[androidManagedStoreAccountAppSyncStatus](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|上次应用程序同步结果。 可取值为：`success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。|
|ownerUserPrincipalName|String|创建了企业的所有者 UPN|
|ownerOrganizationName|String|载入 Android 应用时所使用的Enterprise|
|lastModifiedDateTime|DateTimeOffset|Android 企业设置的上次修改时间|
|enrollmentTarget|[androidManagedStoreAccountEnrollmentTarget](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|指示哪些用户可以在 Android 中注册设备Enterprise设备管理。 可取值为：`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions`。|
|targetGroupIds|String collection|指定当 enrollmentTarget 设置为“定向”时可以在 Android for Work 设备管理中注册设备的 AAD 组。|
|deviceOwnerManagementEnabled|Boolean|指示此帐户是否正在通过 CloudDPC 对 Android 设备所有者管理进行测试。|
|companyCodes|[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) 集合|AndroidManagedStoreAccountEnterpriseSettings 的公司代码|
|androidDeviceOwnerFullyManagedEnrollmentEnabled|Boolean|AndroidManagedStoreAccountEnterpriseSettings 的公司代码|
|managedGooglePlayInitialScopeTagIds|字符串集合|MGP 应用的初始范围标记|

## <a name="relationships"></a>关系
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
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
      "enrollmentToken": "String",
      "qrCodeContent": "String",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "String",
        "value": "binary"
      }
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true,
  "managedGooglePlayInitialScopeTagIds": [
    "String"
  ]
}
```




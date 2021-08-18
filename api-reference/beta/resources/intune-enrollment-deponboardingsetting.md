---
title: depOnboardingSetting 资源类型
description: depOnboardingSetting 表示要载入到 Intune 的 Apple DEP 服务的实例。 载入的服务实例管理用于在 Apple 和 Intune 之间同步数据的 Apple 令牌。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ac9e8c7909d817544141a8a409d434c31d229ded5392376f51266b0532e221ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251244"
---
# <a name="deponboardingsetting-resource-type"></a>depOnboardingSetting 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

depOnboardingSetting 表示要载入到 Intune 的 Apple DEP 服务的实例。 载入的服务实例管理用于在 Apple 和 Intune 之间同步数据的 Apple 令牌。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 depOnboardingSettings](../api/intune-enrollment-deponboardingsetting-list.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) 集合|列出 [depOnboardingSetting 对象的属性和](../resources/intune-enrollment-deponboardingsetting.md) 关系。|
|[获取 depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-get.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|读取 [depOnboardingSetting 对象的属性和](../resources/intune-enrollment-deponboardingsetting.md) 关系。|
|[创建 depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-create.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|创建新的 [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) 对象。|
|[删除 depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-delete.md)|无|删除 [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)。|
|[更新 depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-update.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|更新 [depOnboardingSetting 对象](../resources/intune-enrollment-deponboardingsetting.md) 的属性。|
|[getEncryptionPublicKey 函数](../api/intune-enrollment-deponboardingsetting-getencryptionpublickey.md)|字符串|获取公钥以用于加密 Apple 设备注册计划令牌|
|[generateEncryptionPublicKey 操作](../api/intune-enrollment-deponboardingsetting-generateencryptionpublickey.md)|String|生成公钥以用于加密 Apple 设备注册计划令牌|
|[uploadDepToken 操作](../api/intune-enrollment-deponboardingsetting-uploaddeptoken.md)|无|上载新的设备注册计划令牌|
|[syncWithAppleDeviceEnrollmentProgram 操作](../api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|无|在 Apple 设备注册计划与 Intune 之间同步|
|[shareForSchoolDataSyncService 操作](../api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice.md)|无|尚未记录|
|[unshareForSchoolDataSyncService 操作](../api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice.md)|无|尚未记录|
|[getExpiringVppTokenCount 函数](../api/intune-enrollment-deponboardingsetting-getexpiringvpptokencount.md)|Int32|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID|
|appleIdentifier|String|用于获取当前令牌的 Apple ID。|
|tokenExpirationDateTime|DateTimeOffset|令牌将过期的时间。|
|lastModifiedDateTime|DateTimeOffset|载入服务时。|
|lastSuccessfulSyncDateTime|DateTimeOffset|服务最后一次与 Intune 进行联合时|
|lastSyncTriggeredDateTime|DateTimeOffset|Intune 上次请求同步时。|
|shareTokenWithSchoolDataSyncService|布尔值|是否使用服务启用 Dep 令牌学校数据同步共享。|
|lastSyncErrorCode|Int32|Apple 在上次取消同步期间报告的错误代码。|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md)|获取或设置 Dep 令牌类型。 可取值为：`none`、`dep`、`appleSchoolManager`。|
|tokenName|字符串|Dep 令牌的友好名称|
|syncedDeviceCount|Int32|获取同步的设备计数|
|dataSharingConsentGranted|布尔值|同意与 Apple Dep 服务共享数据|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|defaultIosEnrollmentProfile|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|默认 iOS 注册配置文件|
|defaultMacOsEnrollmentProfile|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|默认 MacOs 注册配置文件|
|enrollmentProfiles|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 集合|注册配置文件。|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) 集合|导入的 Apple 设备标识。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depOnboardingSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastSuccessfulSyncDateTime": "String (timestamp)",
  "lastSyncTriggeredDateTime": "String (timestamp)",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1024,
  "tokenType": "String",
  "tokenName": "String",
  "syncedDeviceCount": 1024,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```





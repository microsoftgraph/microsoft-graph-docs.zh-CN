---
title: depOnboardingSetting 资源类型
description: DepOnboardingSetting 表示正在对 Intune onboarded Apple DEP 服务的实例。 Onboarded 服务实例管理 Apple 令牌用于 Apple 和 Intune 之间同步数据。
ms.openlocfilehash: 7991b03b8307db10d3a300b1b85be3fc1b825819
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048904"
---
# <a name="deponboardingsetting-resource-type"></a>depOnboardingSetting 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

DepOnboardingSetting 表示正在对 Intune onboarded Apple DEP 服务的实例。 Onboarded 服务实例管理 Apple 令牌用于 Apple 和 Intune 之间同步数据。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 depOnboardingSettings](../api/intune-enrollment-deponboardingsetting-list.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)集合|列出属性和[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象之间的关系。|
|[获取 depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-get.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|读取属性和[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象的关系。|
|[创建 depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-create.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|创建新的[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象。|
|[删除 depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-delete.md)|无|删除[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)。|
|[更新 depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-update.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|更新[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象的属性。|
|[getEncryptionPublicKey 函数](../api/intune-enrollment-deponboardingsetting-getencryptionpublickey.md)|字符串|获取要用于加密 Apple 设备注册程序的公钥标记|
|[uploadDepToken 操作](../api/intune-enrollment-deponboardingsetting-uploaddeptoken.md)|无|上载新的设备注册程序令牌|
|[syncWithAppleDeviceEnrollmentProgram 操作](../api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|无|Apple 设备注册程序和 Intune 之间同步|
|[shareForSchoolDataSyncService 操作](../api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice.md)|无|尚未记录|
|[unshareForSchoolDataSyncService 操作](../api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID|
|appleIdentifier|String|Apple ID 用来获取当前的令牌。|
|tokenExpirationDateTime|DateTimeOffset|该令牌将过期时。|
|lastModifiedDateTime|DateTimeOffset|当该服务已 onboarded。|
|lastSuccessfulSyncDateTime|DateTimeOffset|当服务与 Intune 的最后一个 syned|
|lastSyncTriggeredDateTime|DateTimeOffset|当 Intune 上次请求同步。|
|shareTokenWithSchoolDataSyncService|布尔|是否 Dep 令牌共享将启用学校数据同步服务。|
|lastSyncErrorCode|Int32|在最后一个 dep 同步过程中由 Apple 报告的错误代码。|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md)|获取或设置 Dep 标记类型。 可取值为：`none`、`dep`、`appleSchoolManager`。|
|tokenName|字符串|Dep 令牌的友好名称|
|syncedDeviceCount|Int32|获取同步设备计数|
|defaultProfileDisplayName|字符串|获取同步设备计数|
|dataSharingConsentGranted|布尔|授予许可与 Apple Dep 服务共享的数据|

## <a name="relationships"></a>Relationships
|关系|类型|说明|
|:---|:---|:---|
|defaultIosEnrollmentProfile|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|默认 iOS 注册配置文件|
|defaultMacOsEnrollmentProfile|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|默认 MacOs 注册配置文件|
|enrollmentProfiles|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)集合|注册配置文件。|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)集合|导入的 Apple 设备标识。|

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
  "defaultProfileDisplayName": "String",
  "dataSharingConsentGranted": true
}
```






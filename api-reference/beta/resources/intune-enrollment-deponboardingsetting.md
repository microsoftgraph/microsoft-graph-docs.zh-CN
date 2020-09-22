---
title: depOnboardingSetting 资源类型
description: DepOnboardingSetting 表示要载入到 Intune 的 Apple DEP 服务的实例。 载入服务实例管理用于在 Apple 和 Intune 之间同步数据的 Apple 令牌。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 85a5a75a3a6ae0a959cf8f363b67c438e17889bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080234"
---
# <a name="deponboardingsetting-resource-type"></a>depOnboardingSetting 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

DepOnboardingSetting 表示要载入到 Intune 的 Apple DEP 服务的实例。 载入服务实例管理用于在 Apple 和 Intune 之间同步数据的 Apple 令牌。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 depOnboardingSettings](../api/intune-enrollment-deponboardingsetting-list.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) 集合|列出 [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) 对象的属性和关系。|
|[获取 depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-get.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|读取 [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) 对象的属性和关系。|
|[创建 depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-create.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|创建新的 [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) 对象。|
|[删除 depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-delete.md)|无|删除 [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)。|
|[更新 depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-update.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|更新 [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) 对象的属性。|
|[getEncryptionPublicKey 函数](../api/intune-enrollment-deponboardingsetting-getencryptionpublickey.md)|String|获取用于加密 Apple 设备注册计划令牌的公钥|
|[generateEncryptionPublicKey 操作](../api/intune-enrollment-deponboardingsetting-generateencryptionpublickey.md)|String|生成用于加密 Apple 设备注册计划令牌的公钥|
|[uploadDepToken 操作](../api/intune-enrollment-deponboardingsetting-uploaddeptoken.md)|无|上传新的设备注册程序令牌|
|[syncWithAppleDeviceEnrollmentProgram 操作](../api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|无|在 Apple 设备注册计划和 Intune 之间进行同步|
|[shareForSchoolDataSyncService 操作](../api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice.md)|无|尚未记录|
|[unshareForSchoolDataSyncService 操作](../api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice.md)|无|尚未记录|
|[getExpiringVppTokenCount 函数](../api/intune-enrollment-deponboardingsetting-getexpiringvpptokencount.md)|Int32|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID|
|appleIdentifier|String|用于获取当前令牌的 Apple ID。|
|tokenExpirationDateTime|DateTimeOffset|令牌将到期的时间。|
|lastModifiedDateTime|DateTimeOffset|在载入服务时。|
|lastSuccessfulSyncDateTime|DateTimeOffset|服务上次使用 Intune syned 时|
|lastSyncTriggeredDateTime|DateTimeOffset|Intune 上次请求同步时。|
|shareTokenWithSchoolDataSyncService|Boolean|是否启用了与学校数据同步服务的 Dep 令牌共享。|
|lastSyncErrorCode|Int32|上一次 dep 同步期间 Apple 报告的错误代码。|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md)|获取或设置 Dep 令牌类型。 可取值为：`none`、`dep`、`appleSchoolManager`。|
|tokenName|String|Dep 令牌的友好名称|
|syncedDeviceCount|Int32|获取同步的设备计数|
|dataSharingConsentGranted|Boolean|为使用 Apple Dep 服务进行数据共享而授予的同意|
|roleScopeTagIds|String 集合|此实体实例的范围标记列表。|

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







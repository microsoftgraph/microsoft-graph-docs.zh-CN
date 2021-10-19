---
title: androidDeviceOwnerEnrollmentProfile 资源类型
description: 注册配置文件，用于Enterprise Google 的云管理注册 Android 设备。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 41db800f2e14e5806b2354e9b59d95f9249da545
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60489743"
---
# <a name="androiddeviceownerenrollmentprofile-resource-type"></a>androidDeviceOwnerEnrollmentProfile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

注册配置文件，用于Enterprise Google 的云管理注册 Android 设备。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 androidDeviceOwnerEnrollmentProfiles](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-list.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) 集合|列出 [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) 对象的属性和关系。|
|[获取 androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-get.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|读取 [androidDeviceOwnerEnrollmentProfile 对象的属性和](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) 关系。|
|[创建 androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-create.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|创建新的 [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) 对象。|
|[删除 androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-delete.md)|无|删除 [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)。|
|[更新 androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-update.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|更新 [androidDeviceOwnerEnrollmentProfile 对象](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) 的属性。|
|[revokeToken 操作](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken.md)|无|尚未记录|
|[createToken 操作](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accountId|String|注册配置文件隶属的租户 GUID。|
|id|String|注册配置文件的唯一 GUID。|
|displayName|String|注册配置文件的显示名称。|
|说明|String|注册配置文件的说明。|
|enrollmentMode|[androidDeviceOwnerEnrollmentMode](../resources/intune-androidforwork-androiddeviceownerenrollmentmode.md)|使用此注册配置文件的设备注册模式。 可取值为：`corporateOwnedDedicatedDevice`、`corporateOwnedFullyManaged`、`corporateOwnedWorkProfile`、`corporateOwnedAOSPUserlessDevice`、`corporateOwnedAOSPUserAssociatedDevice`。|
|enrollmentTokenType|[androidDeviceOwnerEnrollmentTokenType](../resources/intune-androidforwork-androiddeviceownerenrollmenttokentype.md)|注册配置文件的注册令牌类型。 可取值为：`default`、`corporateOwnedDedicatedDeviceWithAzureADSharedMode`。|
|createdDateTime|DateTimeOffset|注册配置文件的创建日期/时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改注册配置文件的日期/时间。|
|tokenValue|String|为此注册配置文件最新创建的令牌的值。|
|tokenCreationDateTime|DateTimeOffset|最近创建的令牌的创建日期时间。|
|tokenExpirationDateTime|DateTimeOffset|最新创建的令牌的到期日期/时间。|
|enrolledDeviceCount|Int32|已使用此注册配置文件进行注册的 Android 设备总数。|
|enrollmentTokenUsageCount|Int32|已使用当前令牌注册的 AOSP 设备总数。|
|qrCodeContent|String|用于生成此令牌的 QR 码的字符串。|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|用于生成此令牌的 QR 码的字符串。|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。|
|wifiSsid|String|包含 WLAN 登录 ssid 的字符串|
|wifiPassword|String|包含 WLAN 登录密码的字符串|
|wifiSecurityType|[aospWifiSecurityType](../resources/intune-androidforwork-aospwifisecuritytype.md)|包含 WLAN 安全类型的字符串。 可取值为：`none`、`wpa`、`wep`。|
|wifiHidden|Boolean|指示是否已启用隐藏的 wifi 网络的布尔值|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "enrollmentMode": "String",
  "enrollmentTokenType": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenCreationDateTime": "String (timestamp)",
  "tokenExpirationDateTime": "String (timestamp)",
  "enrolledDeviceCount": 1024,
  "enrollmentTokenUsageCount": 1024,
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "roleScopeTagIds": [
    "String"
  ],
  "wifiSsid": "String",
  "wifiPassword": "String",
  "wifiSecurityType": "String",
  "wifiHidden": true
}
```




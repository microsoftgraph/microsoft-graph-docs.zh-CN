---
title: androidForWorkEnrollmentProfile 资源类型
description: 注册配置文件，用于使用 Google 的云管理注册 COSU 设备。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0136b8d81546ad85ef9c0b0a30a1eb95b84c84f1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59106768"
---
# <a name="androidforworkenrollmentprofile-resource-type"></a>androidForWorkEnrollmentProfile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

注册配置文件，用于使用 Google 的云管理注册 COSU 设备。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List androidForWorkEnrollmentProfiles](../api/intune-androidforwork-androidforworkenrollmentprofile-list.md)|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 集合|列出 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 对象的属性和关系。|
|[Get androidForWorkEnrollmentProfile](../api/intune-androidforwork-androidforworkenrollmentprofile-get.md)|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|读取 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 对象的属性和关系。|
|[Create androidForWorkEnrollmentProfile](../api/intune-androidforwork-androidforworkenrollmentprofile-create.md)|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|创建新的 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 对象。|
|[Delete androidForWorkEnrollmentProfile](../api/intune-androidforwork-androidforworkenrollmentprofile-delete.md)|无|删除 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)。|
|[Update androidForWorkEnrollmentProfile](../api/intune-androidforwork-androidforworkenrollmentprofile-update.md)|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|更新 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 对象的属性。|
|[revokeToken 操作](../api/intune-androidforwork-androidforworkenrollmentprofile-revoketoken.md)|无|尚未记录|
|[createToken 操作](../api/intune-androidforwork-androidforworkenrollmentprofile-createtoken.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accountId|String|注册配置文件隶属的租户 GUID。|
|id|String|注册配置文件的唯一 GUID。|
|displayName|String|注册配置文件的显示名称。|
|说明|String|注册配置文件的说明。|
|createdDateTime|DateTimeOffset|注册配置文件的创建日期/时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改注册配置文件的日期/时间。|
|tokenValue|String|为此注册配置文件最新创建的令牌的值。|
|tokenExpirationDateTime|DateTimeOffset|最新创建的令牌的到期日期/时间。|
|enrolledDeviceCount|Int32|已使用此注册配置文件进行注册的 Android 设备总数。|
|qrCodeContent|String|用于生成此令牌的 QR 码的字符串。|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|用于生成此令牌的 QR 码的字符串。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "enrolledDeviceCount": 1024,
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```




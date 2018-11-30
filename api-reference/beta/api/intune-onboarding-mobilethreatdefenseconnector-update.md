---
title: 更新 mobileThreatDefenseConnector
description: 更新 mobileThreatDefenseConnector 对象的属性。
ms.openlocfilehash: 0a7518c2c751c55a89d02c3d67f87d7a272f895d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047161"
---
# <a name="update-mobilethreatdefenseconnector"></a>更新 mobileThreatDefenseConnector

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象的属性。
## <a name="prerequisites"></a>先决条件
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。


|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象的 JSON 表示形式。

下表显示了创建 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|尚未记录|
|lastHeartbeatDateTime|DateTimeOffset|从数据同步合作伙伴接收到上一个检测信号的日期/时间|
|partnerState|[mobileThreatPartnerTenantState](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|数据同步合作伙伴为此帐户的的状态。 可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。|
|androidEnabled|Boolean|对于 Android 设备，设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据|
|iosEnabled|Boolean|对于 iOS 设备，获取或设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据|
|windowsEnabled|布尔|用于 Windows，获取或设置是否法规遵从性评估期间应使用从数据同步合作伙伴的数据|
|macEnabled|布尔|用于 Mac，获取或设置是否法规遵从性评估期间应使用从数据同步合作伙伴的数据|
|androidDeviceBlockedOnMissingPartnerData|Boolean|对于 Android 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据|
|iosDeviceBlockedOnMissingPartnerData|Boolean|对于 iOS 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据|
|windowsDeviceBlockedOnMissingPartnerData|布尔|对于 Windows，设置是否 Intune 必须接收来自之前标记设备符合数据同步合作伙伴的数据|
|macDeviceBlockedOnMissingPartnerData|布尔|用于 Mac，获取或设置是否 Intune 必须接收来自之前标记设备符合数据同步合作伙伴的数据|
|partnerUnsupportedOsVersionBlocked|Boolean|获取或设置是否阻止不符合数据同步合作伙伴最低版本要求的启用平台上的设备|
|partnerUnresponsivenessThresholdInDays|Int32|获取或设置每个租户允许此合作伙伴集成不响应的天数|
|allowPartnerToCollectIOSApplicationMetadata|布尔|对于 IOS 设备，允许管理员配置是否从 Intune 数据同步合作伙伴中可能还收集有关已安装应用程序的元数据|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 555

{
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```






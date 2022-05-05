---
title: 创建 mobileThreatDefenseConnector
description: 创建新的 mobileThreatDefenseConnector 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1a8aa77292f4f1690ecff29783b30a4117e6fa8a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212924"
---
# <a name="create-mobilethreatdefenseconnector"></a>创建 mobileThreatDefenseConnector

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 mobileThreatDefenseConnector 对象的 JSON 表示形式。

下表显示创建 mobileThreatDefenseConnector 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|lastHeartbeatDateTime|DateTimeOffset|从数据同步合作伙伴接收到上一个检测信号的日期/时间|
|partnerState|[mobileThreatPartnerTenantState](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|数据同步此帐户的合作伙伴状态。 可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。|
|androidMobileApplicationManagementEnabled|Boolean|对于 Android，请设置是否应在移动应用程序管理 (MAM) 评估期间使用来自数据同步伙伴的数据。 对于移动应用程序管理 (MAM) 评估，每个平台只能启用一个合作伙伴。|
|iosMobileApplicationManagementEnabled|Boolean|对于 IOS，获取或设置是否应在移动应用程序管理 (MAM) 评估期间使用来自数据同步伙伴的数据。 对于移动应用程序管理 (MAM) 评估，每个平台只能启用一个合作伙伴。|
|androidEnabled|Boolean|对于 Android 设备，设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据|
|iosEnabled|Boolean|对于 iOS 设备，获取或设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据|
|windowsEnabled|Boolean|对于Windows，获取或设置是否应在符合性评估期间使用来自数据同步伙伴的数据|
|macEnabled|Boolean|对于 Mac，获取或设置是否应在符合性评估期间使用来自数据同步伙伴的数据|
|androidDeviceBlockedOnMissingPartnerData|Boolean|对于 Android 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据|
|iosDeviceBlockedOnMissingPartnerData|Boolean|对于 iOS 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据|
|windowsDeviceBlockedOnMissingPartnerData|Boolean|对于Windows，设置Intune是否必须从数据同步伙伴接收数据，然后再标记符合设备的要求|
|macDeviceBlockedOnMissingPartnerData|Boolean|对于 Mac，获取或设置Intune在标记符合设备之前是否必须从数据同步伙伴接收数据|
|partnerUnsupportedOsVersionBlocked|Boolean|获取或设置是否阻止不符合数据同步合作伙伴最低版本要求的启用平台上的设备|
|partnerUnresponsivenessThresholdInDays|Int32|获取或设置每个租户允许此合作伙伴集成不响应的天数|
|allowPartnerToCollectIOSApplicationMetadata|Boolean|对于 IOS 设备，允许管理员配置数据同步伙伴是否也可以从Intune收集有关已安装应用程序的元数据|
|allowPartnerToCollectIOSPersonalApplicationMetadata|Boolean|对于 IOS 设备，允许管理员配置数据同步伙伴是否也可以从Intune收集有关个人安装的应用程序的元数据|
|microsoftDefenderForEndpointAttachEnabled|Boolean|如果为 TRUE，则启用通过Microsoft Defender for Endpoint的配置文件管理。 如果为 FALSE，则禁用通过Microsoft Defender for Endpoint的配置文件管理。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 844

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidMobileApplicationManagementEnabled": true,
  "iosMobileApplicationManagementEnabled": true,
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
  "allowPartnerToCollectIOSApplicationMetadata": true,
  "allowPartnerToCollectIOSPersonalApplicationMetadata": true,
  "microsoftDefenderForEndpointAttachEnabled": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 893

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidMobileApplicationManagementEnabled": true,
  "iosMobileApplicationManagementEnabled": true,
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
  "allowPartnerToCollectIOSApplicationMetadata": true,
  "allowPartnerToCollectIOSPersonalApplicationMetadata": true,
  "microsoftDefenderForEndpointAttachEnabled": true
}
```





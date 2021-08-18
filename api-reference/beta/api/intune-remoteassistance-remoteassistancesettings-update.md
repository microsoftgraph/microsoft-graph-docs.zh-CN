---
title: 更新 remoteAssistanceSettings
description: 更新 remoteAssistanceSettings 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c24451d22786337ff06140bf6f9299f00e5397c
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58263361"
---
# <a name="update-remoteassistancesettings"></a>更新 remoteAssistanceSettings

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [remoteAssistanceSettings 对象](../resources/intune-remoteassistance-remoteassistancesettings.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistanceSettings
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [remoteAssistanceSettings](../resources/intune-remoteassistance-remoteassistancesettings.md) 对象的 JSON 表示形式。

下表显示创建 [remoteAssistanceSettings 时所需的属性](../resources/intune-remoteassistance-remoteassistancesettings.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|远程协助设置标识符|
|remoteAssistanceState|[remoteAssistanceState](../resources/intune-remoteassistance-remoteassistancestate.md)|帐户的远程协助的当前状态。 可能的值包括：notConfigured、disabled、enabled。 管理员可以配置此设置。管理员尚未配置的远程协助设置具有 notConfigured 状态。 默认返回。 可取值为：`notConfigured`、`disabled`、`enabled`。|
|allowSessionsToUnenrolledDevices|布尔值| 指示是否允许帐户使用到注销设备的会话。 管理员可以配置此设置。默认值为 false。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [remoteAssistanceSettings](../resources/intune-remoteassistance-remoteassistancesettings.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteAssistanceSettings
Content-type: application/json
Content-length: 151

{
  "@odata.type": "#microsoft.graph.remoteAssistanceSettings",
  "remoteAssistanceState": "disabled",
  "allowSessionsToUnenrolledDevices": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 200

{
  "@odata.type": "#microsoft.graph.remoteAssistanceSettings",
  "id": "cfef360e-360e-cfef-0e36-efcf0e36efcf",
  "remoteAssistanceState": "disabled",
  "allowSessionsToUnenrolledDevices": true
}
```





---
title: 更新 deviceManagementDomainJoinConnector
description: 更新 deviceManagementDomainJoinConnector 对象的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 95095857e77e5aa27e413690ebbe7253407745ae
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59070081"
---
# <a name="update-devicemanagementdomainjoinconnector"></a>更新 deviceManagementDomainJoinConnector

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [deviceManagementDomainJoinConnector 对象](../resources/intune-odj-devicemanagementdomainjoinconnector.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) 对象的 JSON 表示形式。

下表显示创建 [deviceManagementDomainJoinConnector 时所需的属性](../resources/intune-odj-devicemanagementdomainjoinconnector.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|表示连接器的唯一标识符。|
|displayName|String|连接器显示名称。|
|lastConnectionDateTime|DateTimeOffset|上次连接器与 Intune 联系的时间。|
|state|[deviceManagementDomainJoinConnectorState](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|连接器状态。 可取值为：`active`、`error`、`inactive`。|
|version|String|连接器的版本。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "error",
  "version": "Version value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "77296cf7-6cf7-7729-f76c-2977f76c2977",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "error",
  "version": "Version value"
}
```




---
title: 更新 zebraFotaArtifact
description: 更新 zebraFotaArtifact 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c3af33735b3d683db14b5d2137734abaf0354eb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213135"
---
# <a name="update-zebrafotaartifact"></a>更新 zebraFotaArtifact

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [zebraFotaArtifact 对象的](../resources/intune-androidfotaservice-zebrafotaartifact.md) 属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/zebraFotaArtifacts/{zebraFotaArtifactId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，为 [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) 对象提供 JSON 表示形式。

下表显示了创建 [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|ZebraFotaArtifact 的 ID。|
|deviceModel|String|项目设备模型。|
|osVersion|String|项目 OS 版本。|
|patchVersion|String|项目修补程序版本。|
|boardSupportPackageVersion|String|开发板支持包的版本。|
|releaseNotesUrl|String|项目发行说明 URL。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/zebraFotaArtifacts/{zebraFotaArtifactId}
Content-type: application/json
Content-length: 311

{
  "@odata.type": "#microsoft.graph.zebraFotaArtifact",
  "deviceModel": "Device Model value",
  "osVersion": "Os Version value",
  "patchVersion": "Patch Version value",
  "boardSupportPackageVersion": "Board Support Package Version value",
  "releaseNotesUrl": "https://example.com/releaseNotesUrl/"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 360

{
  "@odata.type": "#microsoft.graph.zebraFotaArtifact",
  "id": "37305f61-5f61-3730-615f-3037615f3037",
  "deviceModel": "Device Model value",
  "osVersion": "Os Version value",
  "patchVersion": "Patch Version value",
  "boardSupportPackageVersion": "Board Support Package Version value",
  "releaseNotesUrl": "https://example.com/releaseNotesUrl/"
}
```





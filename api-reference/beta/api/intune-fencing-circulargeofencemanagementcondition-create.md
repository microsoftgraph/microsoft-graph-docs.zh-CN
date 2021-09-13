---
title: 创建 circularGeofenceManagementCondition
description: 创建新的 circularGeofenceManagementCondition 对象。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56050bc4ebf036f3eaa771189b4167a0688625af
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59065265"
---
# <a name="create-circulargeofencemanagementcondition"></a>创建 circularGeofenceManagementCondition

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) 对象。

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
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 circularGeofenceManagementCondition 对象的 JSON 表示形式。

下表显示创建 circularGeofenceManagementCondition 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|管理条件的唯一标识符。 创建时分配的系统生成值。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|唯一名称|String|管理条件的唯一名称。 在管理条件表达式中使用。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|管理员定义的管理条件名称。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|说明|String|管理员定义的管理条件说明。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|创建管理条件的时间。 生成的服务器端。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|上次修改管理条件的时间。 更新的服务器端。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|管理条件的 ETag。 更新的服务器端。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[devicePlatformType](../resources/intune-fencing-deviceplatformtype.md) 集合|此管理条件的适用平台。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。|
|latitude|Double|纬度（以度数表示），介于 -90 和 +90 之间（含这两者）。|
|longitude|Double|以度数表示的经度，介于 -180 和 +180 之间（含这两者）。|
|radiusInMeters|单一|以米为单位的半径。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": 2.6666666666666665,
  "longitude": 3.0,
  "radiusInMeters": 4.666666666666667
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "id": "30ee27b6-27b6-30ee-b627-ee30b627ee30",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": 2.6666666666666665,
  "longitude": 3.0,
  "radiusInMeters": 4.666666666666667
}
```




---
title: 更新 appleUserInitiatedEnrollmentProfile
description: 更新 appleUserInitiatedEnrollmentProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3268ffc8dce7e31560cf2db97f146c4b5eb3f071
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60494442"
---
# <a name="update-appleuserinitiatedenrollmentprofile"></a>更新 appleUserInitiatedEnrollmentProfile

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [appleUserInitiatedEnrollmentProfile 对象](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) 的属性。

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
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) 对象的 JSON 表示形式。

下表显示创建 [appleUserInitiatedEnrollmentProfile 时所需的属性](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)。

|属性|类型|说明|
|:---|:---|:---|
|defaultEnrollmentType|[appleUserInitiatedEnrollmentType](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|默认配置文件注册类型。 可取值为：`unknown`、`device`、`user`。|
|availableEnrollmentTypeOptions|[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) 集合|可用注册类型选项列表|
|id|String|对象的 GUID|
|displayName|String|配置文件的名称|
|说明|String|配置文件的说明|
|priority|Int32|优先级，0 为最高|
|平台|[devicePlatformType](../resources/intune-enrollment-deviceplatformtype.md)|设备平台。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`、`androidAOSP`。|
|createdDateTime|DateTimeOffset|配置文件创建时间|
|lastModifiedDateTime|DateTimeOffset|配置文件上次修改时间|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
Content-type: application/json
Content-length: 439

{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "device",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "company",
      "enrollmentType": "device"
    }
  ],
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "platform": "androidForWork"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "device",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "company",
      "enrollmentType": "device"
    }
  ],
  "id": "5a11d98e-d98e-5a11-8ed9-115a8ed9115a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "platform": "androidForWork",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




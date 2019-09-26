---
title: 创建 mobileAppDependency
description: 创建新的 mobileAppDependency 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 321fb11e5e1ee977facd0649c87ef0e46c717b59
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37177078"
---
# <a name="create-mobileappdependency"></a>创建 mobileAppDependency

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 mobileAppDependency 对象的 JSON 表示形式。

下表显示创建 mobileAppDependency 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|关系实体 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|String|目标子移动应用程序的应用程序 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|String|目标子移动应用程序的显示名称。 继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|dependencyType|[mobileAppDependencyType](../resources/intune-apps-mobileappdependencytype.md)|父应用和子应用之间的依赖关系的类型。 可取值为：`detect`、`autoInstall`。|
|dependentAppCount|Int32|子应用程序的依赖项总数。|



## <a name="response"></a>响应
如果成功，此方法在响应`201 Created`正文中返回响应代码和[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```





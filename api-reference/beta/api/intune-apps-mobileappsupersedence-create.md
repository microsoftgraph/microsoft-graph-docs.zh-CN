---
title: 创建 mobileAppSupersedence
description: 创建新的 mobileAppSupersedence 对象。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2c2e740004b91b949656e3b1c7a29085ea4f88a5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59061968"
---
# <a name="create-mobileappsupersedence"></a>创建 mobileAppSupersedence

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
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
在请求正文中，提供 mobileAppSupersedence 对象的 JSON 表示形式。

下表显示创建 mobileAppSupersedence 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|关系实体 ID。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|String|目标移动应用的应用 ID。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|String|目标移动应用显示名称。 继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayVersion|String|目标移动应用的显示版本。 继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetPublisher|String|目标移动应用的发布者。 继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|关系类型，指示目标是父对象还是子级。 继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)。 可取值为：`child`、`parent`。|
|supersedenceType|[mobileAppSupersedenceType](../resources/intune-apps-mobileappsupersedencetype.md)|父应用和子应用之间的取代关系类型。 可取值为：`update`、`replace`。|
|supersededAppCount|Int32|被子应用直接或间接取代的应用总数。|
|supersedingAppCount|Int32|直接或间接取代父应用的应用总数。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 424

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "id": "c0254204-4204-c025-0442-25c0044225c0",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```




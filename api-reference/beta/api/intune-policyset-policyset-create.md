---
title: 创建 policySet
description: 创建新的 policySet 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d12d43cf0f4da721ef5361fe94aa845134f1c6a1668fd20449f6d3a1f18747e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54207759"
---
# <a name="create-policyset"></a>创建 policySet

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [policySet](../resources/intune-policyset-policyset.md) 对象。

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
POST /deviceAppManagement/policySets
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 policySet 对象的 JSON 表示形式。

下表显示创建 policySet 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|PolicySet 的键。|
|createdDateTime|DateTimeOffset|PolicySet 的创建时间。|
|lastModifiedDateTime|DateTimeOffset|PolicySet 的上次修改时间。|
|displayName|字符串|PolicySet 的 DisplayName。|
|description|String|PolicySet 的说明。|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|PolicySet 的验证/分配状态。 可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|错误代码（如果发生了任何错误）。 可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。|
|guidedDeploymentTags|String collection|引导式部署的标记|
|roleScopeTags|String collection|PolicySet 的 RoleScopeTags|



## <a name="response"></a>响应
如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [policySet](../resources/intune-policyset-policyset.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.policySet",
  "displayName": "Display Name value",
  "description": "Description value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.policySet",
  "id": "653cb373-b373-653c-73b3-3c6573b33c65",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```





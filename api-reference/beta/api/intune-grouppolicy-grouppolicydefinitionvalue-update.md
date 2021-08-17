---
title: 更新 groupPolicyDefinitionValue
description: 更新 groupPolicyDefinitionValue 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 793a3675be699b94da47555b0c644c4540e24b5b5faac16cf0c789c98f4f8abe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54158774"
---
# <a name="update-grouppolicydefinitionvalue"></a>更新 groupPolicyDefinitionValue

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [groupPolicyDefinitionValue 对象](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) 的属性。

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
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) 对象的 JSON 表示形式。

下表显示创建 [groupPolicyDefinitionValue 时所需的属性](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)。

|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|对象的创建日期和时间。|
|enabled|Boolean|启用或禁用关联的组策略定义。|
|configurationType|[groupPolicyConfigurationType](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|指定值配置方式。 它可以作为策略或首选项。 可能的值是：`policy`、`preference`。|
|id|String|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "enabled": true,
  "configurationType": "preference",
  "id": "50428918-8918-5042-1889-425018894250",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





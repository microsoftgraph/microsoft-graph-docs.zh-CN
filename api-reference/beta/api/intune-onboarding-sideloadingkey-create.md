---
title: 创建 sideLoadingKey
description: 创建新的 sideLoadingKey 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 178236e03d508eb8a5017b67a1795fceca72bdee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838869"
---
# <a name="create-sideloadingkey"></a>创建 sideLoadingKey

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

创建新的[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象。
## <a name="prerequisites"></a>先决条件
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。


|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 sideLoadingKey 对象的 JSON 表示形式。

下表显示时创建 sideLoadingKey 所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|端加载关键的唯一 id。|
|值|字符串|端加载密钥值是 5x5 的值，通过 hiphens 分隔。|
|displayName|字符串|端加载项显示名称为 it 专业人员管理员。|
|说明|字符串|显示为 it 专业人员 Admins 端加载项说明正在|
|totalActivation|Int32|端加载项总激活向 it 专业人员 Admins 显示。|
|lastUpdatedDateTime|字符串|端加载项上次更新日期向 it 专业人员 Admins 显示。|



## <a name="response"></a>响应
如果成功，此方法返回`201 Created`响应代码和响应正文中的[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```






---
title: 创建 cloudPcUserSetting
description: 创建新的 cloudPcUserSetting 。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: de9c9418796189b0f4d56f69672cd0c61f3da7b9
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993648"
---
# <a name="create-cloudpcusersetting"></a>创建 cloudPcUserSetting

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|CloudPC.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/userSettings
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                |
| :------------ | :------------------------  |
| Authorization | Bearer {token}。必需。  |
| Content-Type  | application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象的 JSON 表示形式。

下表显示创建 [cloudPcUserSetting](../resources/cloudpcusersetting.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|显示在 UI 中的设置名称。 |
|localAdminEnabled|布尔|若要启用本地管理员选项，将此设置更改为 `True` 。  |
|selfServiceEnabled|布尔|若要启用自助服务选项，将此设置更改为 `True` 。 |
|lastModifiedDateTime|DateTimeOffset|上次修改设置的日期和时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_cloudpcusersetting_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings
Content-Type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "displayName": "Example",
  "selfServiceEnabled": false,
  "localAdminEnabled": true
}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcUserSetting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "id": "556092f8-92f8-5560-f892-6055f8926055",
  "displayName": "Example",
  "selfServiceEnabled": false,
  "localAdminEnabled": true,
  "lastModifiedDateTime": "2021-02-01T10:29:57Z"  
}
```


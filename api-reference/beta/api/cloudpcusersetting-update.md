---
title: 更新 cloudPcUserSetting
description: 更新 cloudPcUserSetting 对象的属性。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: f6e6d6618e4bc90d23c0b3ec552026953a82bfb9
ms.sourcegitcommit: 0fa7148e0b776663eaca3e79e72b85046d4b8b1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/15/2022
ms.locfileid: "63500929"
---
# <a name="update-cloudpcusersetting"></a>更新 cloudPcUserSetting

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [cloudPcUserSetting 对象](../resources/cloudpcusersetting.md) 的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|CloudPC.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                |
| :------------ | :------------------------  |
| Authorization | Bearer {token}。必需。  |
| Content-Type  | application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象的 JSON 表示形式。

下表显示更新 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|用户界面中显示的设置名称。|
|localAdminEnabled|Boolean|若要启用本地管理员选项，将此设置更改为 `True`。  |
|selfServiceEnabled|Boolean|若要启用自助服务选项，将此设置更改为 `True`。 |
|restorePointSetting|[cloudPcRestorePointSetting](../resources/cloudpcrestorepointsetting.md)|定义创建还原点的频率 (即，为用户预配的云电脑拍摄) 快照 (默认值为 12 小时) ，以及是否允许用户将自己的云电脑还原到特定时间点的备份。|
|lastModifiedDateTime|DateTimeOffset|上次修改设置的日期和时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。 |



## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_cloudpcusersetting"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "displayName": "Example",
  "selfServiceEnabled": true,
  "restorePointSetting": {
    "frequencyInHours": 16,
    "userRestoreEnabled": true
  },
  "localAdminEnabled": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-cloudpcusersetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-cloudpcusersetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-cloudpcusersetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-cloudpcusersetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-cloudpcusersetting-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-cloudpcusersetting-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

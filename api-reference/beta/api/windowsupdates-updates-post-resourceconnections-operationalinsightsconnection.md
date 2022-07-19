---
title: 创建 operationalInsightsConnection
description: 创建新的 operationalInsightsConnection 对象。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 85990438cec500e8c7f45c08ee1fe907f1f97efc
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856555"
---
# <a name="create-operationalinsightsconnection"></a>创建 operationalInsightsConnection
命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|WindowsUpdates.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|WindowsUpdates.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/resourceConnections
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) 对象的 JSON 表示形式。

创建 **operationalInsightsConnection** 时，必须指定以下属性。

|属性|类型|Description|
|:---|:---|:---|
|azureResourceGroupName|String|包含 Log Analytics 工作区的 Azure 资源组的名称。|
|azureSubscriptionId|字符串|包含 Log Analytics 工作区的 Azure 订阅 ID。|
|workspaceName|String|Log Analytics 工作区的名称。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) 对象。

可能会出现以下错误：

|响应代码|邮件|
|:---|:---|
|`400 Bad Request`|指定的工作区无法链接。 验证密钥属性是否正确。|
|`403 Forbidden`|指定的工作区无法链接。 验证 Azure 订阅是否处于活动状态。|
|`409 Conflict`|指定的资源已存在。|

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "create_operationalInsightsConnection_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/resourceConnections
Content-Type: application/json
Content-length: 97

{
  "@odata.type": "#microsoft.graph.windowsUpdates.operationalInsightsConnection",
  "azureSubscriptionId": "322ec614-e9c2-4cd5-a55c-5711fdecf02e",
  "azureResourceGroupName": "target-resource-group",
  "workspaceName": "my-workspace"
}
```


### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.operationalInsightsConnection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.operationalInsightsConnection",
  "id": "85fbecb2-e407-34e9-9298-4d587857795d",
  "azureSubscriptionId": "322ec614-e9c2-4cd5-a55c-5711fdecf02e",
  "azureResourceGroupName": "target-resource-group",
  "workspaceName": "my-workspace",
  "state": "connected"
}
```
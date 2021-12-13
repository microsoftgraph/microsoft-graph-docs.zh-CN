---
title: 创建linkedResource_v2
description: 创建新的 linkedResource_v2 对象。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c16eb6927367b13cc8d0cdad5d5e815f3e758139
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424833"
---
# <a name="create-linkedresource_v2"></a>创建linkedResource_v2
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [linkedResource_v2](../resources/linkedresource_v2.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Tasks.ReadWrite|
|委派（个人 Microsoft 帐户）|Tasks.ReadWrite|
|Application|Tasks.ReadWrite|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/tasks/lists/{baseTaskListId}/tasks/{baseTaskId}/linkedResources
POST /users/{id | userPrincipalName}/tasks/lists/{baseTaskListId}/tasks/{baseTaskId}/linkedResources
```
## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 linkedResource_v2 [对象的 JSON](../resources/linkedresource_v2.md) 表示形式。

在创建一个属性时，**可以指定linkedResource_v2。**

|属性|类型|说明|
|:---|:---|:---|
|applicationName|String|指示发送 **linkedResource** 的源的应用名称的字段。|
|displayName|字符串|指示 **linkedResource 的标题的字段**。|
|externalId|String|第三方/合作伙伴系统上与此任务关联的对象的 ID。|
|WebUrl|String|指向 **linkedResource 的深层链接**。|

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码 [linkedResource_v2](../resources/linkedresource_v2.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_linkedresource_v2_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/tasks/lists/AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA/linkedResources
Content-Type: application/json

{
    "webUrl": "https://microsoft.com",
    "applicationName": "Microsoft",
    "displayName": "Microsoft",
    "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource_v2"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('6f9a2a92-8527-4d64-937e-b5312852f35d')/tasks/lists('AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA%3D')/tasks('AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA')/linkedResources/$entity",
    "webUrl": "https://microsoft.com",
    "applicationName": "Microsoft",
    "displayName": "Microsoft",
    "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9",
    "id": "e2c5ed75-7aa4-4f8e-84ab-98b5e0b56ee8"
}
```


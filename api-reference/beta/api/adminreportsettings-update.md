---
title: 更新 adminReportSettings
description: 更新 Microsoft 365 报表的租户级别设置。
ms.localizationpriority: medium
author: qiwhuang
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 0fb9ed8d8e80bf195e3d63f5139ca6498246fc48
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856556"
---
# <a name="update-adminreportsettings"></a>更新 adminReportSettings

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 Microsoft 365 报表的租户级别设置。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|----------------------------------------|---------------------------------------------|
| 委派（工作或学校帐户）     | ReportSettings.ReadWrite.All                |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用程序                            | ReportSettings.ReadWrite.All                |

> **注意：** 对于允许应用代表用户更新报表设置的委派权限，租户管理员必须为用户分配相应的 Azure Active Directory 受限管理员角色。 有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } --> 
```http
PATCH /admin/reportSettings
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                |
| :------------ | :--------------------------|
| Authorization | Bearer {token}。必需。  |
| Content-Type  | application/json. Required.|

## <a name="request-body"></a>请求正文

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| 属性       | 类型           | Description                                 |
| -------------- | -------------- | ------------------------------------------- |
| displayConcealedNames | Boolean | 如果设置为 `true`，所有报表都将隐藏用户名、组和网站等用户信息。 如果 `false`，所有报表都将显示可识别的信息。 此属性表示Microsoft 365 管理中心中的设置。 必需。 |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

下面是更新 Microsoft 365 报表的租户级别设置的请求示例。

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "update_adminreportsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/reportSettings
Content-Type: application/json
Content-length: 37

{
  "displayConcealedNames": true
}
```

### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

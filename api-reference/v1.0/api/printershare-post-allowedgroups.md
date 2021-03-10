---
title: 为 printerShare 创建 allowedGroup
description: 授予指定的组访问权限，以将打印作业提交到关联的打印机。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 8db8facb302863ec96107c333b8e17f59f2b27a4
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573857"
---
# <a name="create-allowedgroup-for-printershare"></a>为 printerShare 创建 allowedGroup
命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

授予指定的组访问权限，以将打印作业提交到关联的[printerShare。](../resources/printershare.md)

## <a name="permissions"></a>权限
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。

若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。 登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| PrinterShare.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|
|Application|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/shares/{printerShareId}/allowedGroups/$ref
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，使用格式提供对组实体的引用， `@odata.id` 如以下示例所示。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_group_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedGroups/$ref
Content-Type: application/json
Content-length: 47

{
  "@odata.id": "https://graph.microsoft.com/v1.0/groups/{groupId}"
}
```


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
}
-->
``` http
HTTP/1.1 204 No Content
```


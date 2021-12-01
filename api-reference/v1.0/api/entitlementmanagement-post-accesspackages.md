---
title: 创建 accessPackage
description: 创建新的 accessPackage。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e9c62d3444f65f0d17dadc26070ffe8afe18eb7d
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242219"
---
# <a name="create-accesspackage"></a>创建 accessPackage

命名空间：microsoft.graph

创建新的 [accessPackage](../resources/accesspackage.md) 对象。

访问包将添加到现有的 [accessPackageCatalog](../resources/accesspackagecatalog.md)。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | 持有者 \{token\}。必需。 |
| Content-type  | application/json. Required.  |

## <a name="request-body"></a>请求正文
在请求正文中，提供 [accessPackage](../resources/accesspackage.md) 对象的 JSON 表示形式。

可以在创建 **accessPackage** 时指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|访问显示名称的组。|
|description|String|访问包的说明。|
|IsHidden|布尔值|访问包是否对请求程序隐藏。|



## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和新 [accessPackage](../resources/accesspackage.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_accesspackage"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackages
Content-Type: application/json

{
  "displayName": "sales reps",
  "description": "outside sales representatives",
  "isHidden": false,
  "catalog": {
    "id": "66584aae-98bb-48cc-9458-7bee5d2a6577"
  }
}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "642181f0-bc17-4fc6-9ebb-ff53dbf18c2f",
  "displayName": "sales reps",
  "description": "outside sales representatives",
  "isHidden": false,
  "createdDateTime": "2021-11-10T01:10:09.5220119Z",
  "modifiedDateTime": "2021-11-10T01:10:09.5220119Z"
}
```


---
title: 创建 managementConditionStatement
description: 创建新的 managementConditionStatement 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: da085e2aa384e2ee3d4eedd611cfe14945b8fe1d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806438"
---
# <a name="create-managementconditionstatement"></a>创建 managementConditionStatement

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

创建新的[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象。
## <a name="prerequisites"></a>先决条件
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。


|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 managementConditionStatement 对象的 JSON 表示形式。

下表显示时创建 managementConditionStatement 所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|管理条件语句的唯一标识符。 系统生成时创建分配值。|
|displayName|字符串|管理员定义管理条件语句的名称。|
|说明|字符串|管理员定义管理条件语句的说明。|
|createdDateTime|DateTimeOffset|创建管理条件语句的时间。 生成的服务方。|
|modifiedDateTime|DateTimeOffset|管理条件语句上次修改时间。 更新服务端。|
|表达式|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|用来评估如果管理条件语句的管理条件语句表达式已激活/停用。|
|eTag|String|管理条件语句的 ETag。 更新服务端。|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合|此管理条件语句适用的平台。
这从查找管理相关的管理条件计算条件语句并查找适用平台的交点。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。|



## <a name="response"></a>响应
如果成功，此方法返回`201 Created`响应代码和响应正文中的[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 491

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```






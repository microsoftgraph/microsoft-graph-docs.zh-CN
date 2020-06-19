---
title: enableUnlicensedAdminstrators 操作
description: 启用后，通过角色分配成员身份分配给管理员的用户将不再需要分配的 Intune 许可证。 对于角色分配中的每个 AAD 安全组，限制为350个无许可证的直接成员，但如果需要支持超过350个未获得授权的管理员，则可以将多个 AAD 安全组分配给一个角色。 许可管理员将继续按中的顺序工作，这是可传递的成员资格应用且不受350成员限制的限制。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 882a5d1cafa8e25d4a69a0c525c0bb8d3b971cd1
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792804"
---
# <a name="enableunlicensedadminstrators-action"></a>enableUnlicensedAdminstrators 操作

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

启用后，通过角色分配成员身份分配给管理员的用户将不再需要分配的 Intune 许可证。 对于角色分配中的每个 AAD 安全组，限制为350个无许可证的直接成员，但如果需要支持超过350个未获得授权的管理员，则可以将多个 AAD 安全组分配给一个角色。 许可管理员将继续按中的顺序工作，这是可传递的成员资格应用且不受350成员限制的限制。

## <a name="prerequisites"></a>先决条件
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableUnlicensedAdminstrators
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableUnlicensedAdminstrators
```

### <a name="response"></a>响应
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
``` http
HTTP/1.1 204 No Content
```




---
title: enableUnlicensedAdminstrators 操作
description: 启用后，通过角色分配成员身份分配给管理员的用户将不再需要分配的 Intune 许可证。 对于角色分配中的每个 AAD 安全组，限制为350个无许可证的直接成员，但如果需要支持超过350个未获得授权的管理员，则可以将多个 AAD 安全组分配给一个角色。 许可管理员将继续按中的顺序工作，这是可传递的成员资格应用且不受350成员限制的限制。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5258e04ba10c0c9c130fb1fae8ce589906f3c870
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706749"
---
# <a name="enableunlicensedadminstrators-action"></a>enableUnlicensedAdminstrators 操作

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

启用后，通过角色分配成员身份分配给管理员的用户将不再需要分配的 Intune 许可证。 对于角色分配中的每个 AAD 安全组，限制为350个无许可证的直接成员，但如果需要支持超过350个未获得授权的管理员，则可以将多个 AAD 安全组分配给一个角色。 许可管理员将继续按中的顺序工作，这是可传递的成员资格应用且不受350成员限制的限制。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

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
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 204 No Content
```






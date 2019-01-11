---
title: 重置 sync educationSynchronizationProfile 上
description: 重置为租户中的特定学校数据同步配置文件同步。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 54352d29280d671aaddc152307d8669f64c11bdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808538"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a>重置 sync educationSynchronizationProfile 上

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

重置为租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)同步。

> **注意：** 此操作将导致同步重新启动。 遇到的任何错误都将被删除。 将从 Azure Active Directory (Azure AD) 中不删除任何数据。 

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | Permissions |
|:-----------|:----------|
| 委派（工作或学校帐户） | EduAdministration.ReadWrite |
|委派 （个人 Microsoft 帐户|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法返回 `200 OK` 响应代码。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a>响应

没有响应正文。

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```

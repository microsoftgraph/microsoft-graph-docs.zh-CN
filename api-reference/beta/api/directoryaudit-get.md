---
title: 获取 directoryAudit
description: 提供 （或获取） 特定的 Azure Active Directory 审核日志项。 包括用户、 应用程序、 设备和组管理、 特权标识管理、 访问评论、 使用条款、 标识保护、 密码管理 （SSPR 和管理密码重置的 Azure Active Directory 中的各种服务所生成的审核日志)，自助服务组管理等...
localization_priority: Normal
ms.openlocfilehash: e85c0c14e4f6c6a0aa3b8beca1ef9d05f4b82aa0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809266"
---
# <a name="get-directoryaudit"></a>获取 directoryAudit
提供 （或获取） 特定的 Azure Active Directory 审核日志项。 包括用户、 应用程序、 设备和组管理、 特权标识管理、 访问评论、 使用条款、 标识保护、 密码管理 （SSPR 和管理密码重置的 Azure Active Directory 中的各种服务所生成的审核日志)，自助服务组管理等...

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AuditLog.Read.All |
|委派（个人 Microsoft 帐户） | 不支持   |
|应用程序 | AuditLog.Read.All | 

此外，应用程序必须采用到 Azure AD 中[正确注册](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/directoryAudits/{id}
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持以下 OData 查询参数，有助于自定义响应。 查看有关如何使用这些参数的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应正文中的响应代码和[directoryAudit](../resources/directoryaudit.md)对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/directoryAudits/{id}
```
##### <a name="response"></a>响应
下面是一个响应示例。 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218
```
```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/directoryAudits
  "value": [{
        "id": "id",
        "category": "UserManagement",
        "correlationId": "dax59xfb-5xfa-4x92-8x38-6e1fx7870e30",
        "result": "success",
        "resultReason": "Successfully added member to group",
        "activityDisplayName": "Add member to group",
        "activityDateTime": "2018-01-09T21:20:02.7215374Z",
        "loggedByService": "Core Directory",
        "initiatedBy": {
            "user": {
                "id": "72xx09ae-1x37-49x7-9xfe-e3xx964db09b",
                "displayName": "Jamie Doe",
                "userPrincipalName": "jdoe@wingtiptoysonline.com",
                "ipAddress": "127.0.0.1"
            },
            "app": null
        },
        "targetResources": [{
            "@odata.type": "#microsoft.graph.TargetResourceGroup",
            "id": "ef7x527d-6xx2-4xx4-8xxd-cxxfdxx5xx95",
            "displayName": "Lynda.com",
            "modifiedProperties": [{
                "displayName": "Action Client Name",
                "oldValue": null,
                "newValue": "DirectorySync"
            }],
            "groupType": "unifiedGroups"
        }, {
            "@odata.type": "#microsoft.graph.targetResourceUser",
            "id": "1x0exxf5-3xx1-4xxb-9xx0-d4xx572xxbb7",
            "displayName": null,
            "modifiedProperties": [],
            "userPrincipalName": "jdoe@contoso.com"
        }],
        "additionalDetails": [{
            "key": "Additional Detail Name",
            "value": "Additional Detail Value"
        }]
    }]
}
```

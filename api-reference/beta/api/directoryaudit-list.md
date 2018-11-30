---
title: 列表 directoryAudits
description: 提供了生成的 Azure Active Directory 的审核日志的列表。 包括用户、 应用程序、 设备和组管理、 特权标识管理、 访问评论、 使用条款、 标识保护、 密码管理 （SSPR 和管理密码重置的 Azure Active Directory 中的各种服务所生成的审核日志)，自助服务组管理等...
ms.openlocfilehash: e607d866443a07f1405260b02a630276951ce310
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041357"
---
# <a name="list-directoryaudits"></a>列表 directoryAudits

提供了生成的 Azure Active Directory 的审核日志的列表。 包括用户、 应用程序、 设备和组管理、 特权标识管理、 访问评论、 使用条款、 标识保护、 密码管理 （SSPR 和管理密码重置的 Azure Active Directory 中的各种服务所生成的审核日志)，自助服务组管理等...

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
GET /auditLogs/directoryAudits
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持以下 OData 查询参数，有助于自定义响应。 查看有关如何使用这些参数的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。

|名称     |说明                            |示例|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](/graph/query-parameters#filter-parameter)|筛选结果（行）。 |/`auditLogs/directoryAudits?&$filter=createdDateTime le 2018-01-24`
|[$top](/graph/query-parameters#top-parameter)|设置结果的页面大小。|`/auditLogs/directoryAudits?$top=1`|
|[$skiptoken](/graph/query-parameters#skiptoken-parameter)|检索下一步页的结果的结果集跨越多个页面。|`auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a>支持的 $filter 参数属性的列表
|属性名称 |支持的运算符|
|:----------------|:------|
|activityDisplayName| eq startswith|
|activityDateTime| eq，ge，le|
|loggedByService|eq|
|initiatedBy/用户/id|eq|
|initiatedBy/用户/displayName| eq|
|userprincipalname 属性 initiatedBy/用户| eq startswith|
|应用程序 initiatedBy/应用程序标识| eq|
|initiatedBy/应用程序/appDisplayName| eq|
|targetResources/any(t: t/id)| eq|
|targetResources/any(t:t/displayName)| eq startswith|
## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应代码和响应正文中的[directoryAudit](../resources/directoryaudit.md)对象的集合。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "get_directoryaudits"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/directoryAudits
```
##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 271
```
```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/directoryAudits
  "value": [{
        "id": "id",
        "category": "UserManagement",
        "correlationId": "da159bfb-54fa-4092-8a38-6e1fa7870e30",
        "result": "success",
        "resultReason": "Successfully added member to group",
        "activityDisplayName": "Add member to group",
        "activityDateTime": "2018-01-09T21:20:02.7215374Z",
        "loggedByService": "Core Directory",
        "initiatedBy": {
            "user": {
                "id": "7283X9ae-1a37-4937-9aex-e35d964db09b",
                "displayName": "Jamie Doe",
                "userPrincipalName": "jdoe@wingtiptoysonline.com",
                "ipAddress": "127.0.0.1"
            },
            "app": null
        },
        "targetResources": [{
            "@odata.type": "#microsoft.graph.TargetResourceGroup",
            "id": "ef7x527d-6x92-42x4-8x6d-cfxfdfx57f95",
            "displayName": "Lynda.com",
            "modifiedProperties": [{
                "displayName": "Action Client Name",
                "oldValue": null,
                "newValue": "DirectorySync"
            }],
            "groupType": "unifiedGroups"
        }, {
            "@odata.type": "#microsoft.graph.targetResourceUser",
            "id": "1f0ex8f5-3x61-4x6b-9x50-d4xx572f2bb7",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryAudits",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
---
title: 列出用户拥有的已删除项目
description: '检索指定用户拥有的最近删除的项目的列表。  '
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7c947d6ebb8a1f268728c07be64451e230497fb6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434473"
---
# <a name="list-deleted-items-owned-by-a-user"></a>列出用户拥有的已删除项目

命名空间：microsoft.graph

检索指定用户拥有的最近删除的项目的列表。  

目前，仅用户拥有的应用程序和组资源支持列表已删除[](../resources/application.md)的项目功能[](../resources/group.md)。

这是一项服务操作，这意味着它不支持分页。  API 最多返回 1，000 个已删除对象，这些对象由用户拥有，按 ID 排序。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
| --- | --- |
| 委派（工作或学校帐户） | Group.Read.All、Group.ReadWrite.All |
| 委派（个人 Microsoft 帐户） |  不支持。 |
| 应用程序 | Group.Read.All、Group.ReadWrite.All  |

## <a name="http-request"></a>HTTP 请求

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| ------------- | ------------------------- |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

请求正文需要以下参数：

| 参数    | 类型 |描述|
|:---------------|:--------|:----------|
|userId|String|所有者的 ID。|
|type|String|要返回的拥有对象的类型; `Group` 当前是唯一受支持的值。|


## <a name="response"></a>响应

成功的请求返回 `200 OK` 响应代码;响应对象包括 ([已删除) ](../resources/directory.md) 目录。

## <a name="example"></a>示例

##### <a name="request"></a>请求

下面是一个请求示例。

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a>响应

下面是一个响应示例。 注意：为了简洁起见，可能会截断此响应对象。 所有支持的属性都从实际调用中返回。

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```

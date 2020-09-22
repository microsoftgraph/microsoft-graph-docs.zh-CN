---
title: 列出用户拥有的已删除项目
description: '检索指定用户拥有的最近删除的项目的列表。  '
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 84d0c9d688ef67fa36354c4cc037ecb61777eb0d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008916"
---
# <a name="list-deleted-items-owned-by-a-user"></a>列出用户拥有的已删除项目

命名空间：microsoft.graph

检索指定用户拥有的最近删除的项目的列表。  

目前，列出已删除项目仅支持用户拥有的 [应用程序](../resources/application.md) 和 [组](../resources/group.md) 资源的功能。

这是一个服务操作，这意味着它不支持分页。  API 返回最大为1000个已删除的对象，这些对象归用户所有，按 ID 排序。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。

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

请求正文需要以下参数：

| 参数    | 类型 |描述|
|:---------------|:--------|:----------|
|userId|String|所有者的 ID。|
|type|String|要返回的所拥有的对象的类型; `group` 目前是唯一受支持的值。|


## <a name="response"></a>响应

成功的请求返回 `200 OK` 响应代码; response 对象包括 [目录 (删除的项) ](../resources/directory.md) 属性。

## <a name="example"></a>示例

##### <a name="request"></a>请求

下面是一个请求示例。

``` http
POST https://graph.microsoft.com/beta/directory/deletedItems/getUserOwnedObjects
Content-type: application/json

{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a>响应

下面是一个响应示例。 注意：为简洁起见，可能会截断此响应对象。 所有受支持的属性都从实际调用返回。

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": "2018-04-01T12:39:16Z",
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





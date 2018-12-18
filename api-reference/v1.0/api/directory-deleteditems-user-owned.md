---
title: 权限
description: '检索列表的、 由指定用户拥有的最近已删除项目。  '
author: lleonard-msft
ms.openlocfilehash: 9ce487d957f4bdaa2684d00865aeac7ea293ad67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351168"
---
# <a name="list-deleted-items-owned-by-a-user"></a>**由用户拥有的删除列表项**

检索列表的、 由指定用户拥有的最近已删除项目。  

目前，删除列表项功能的用户所拥有的[group](../resources/group.md)资源仅支持。

这是服务操作，这意味着它不支持分页。  API 返回多达 1,000 个用户，按 ID 排序所拥有的已删除的对象

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

| Name          | 说明               |
| ------------- | ------------------------- |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

在请求正文需要以下参数：

| 参数    | Type |说明|
|:---------------|:--------|:----------|
|userId|String|所有者的 ID。|
|type|字符串|要返回; 的拥有对象的类型`Group`目前唯一受支持的值。|


## <a name="response"></a>响应

成功的请求返回`200 OK`响应代码;响应对象包含[目录 （已删除项）](../resources/directory.md)的属性。

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

下面是一个响应示例。 注意： 为了简单起见，此响应对象可能被截断。 从实际的调用返回所有支持的属性。

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



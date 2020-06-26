---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: 获取帐户的 OneDrive 使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0191f4cce6690a77b9c9f9176c47e30c70a6fc4c
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896747"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a>reportRoot: getOneDriveUsageAccountDetail

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取帐户的 OneDrive 使用情况的详细信息。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 报表-OneDrive For business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。

## <a name="permissions"></a>权限

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :--------------------------------------- |
| 委派（工作或学校帐户）     | Reports.Read.All                         |
| 委派（个人 Microsoft 帐户） | 不支持。                           |
| 应用                            | Reports.Read.All                         |

**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。 有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a>函数参数

在请求 URL 中，提供以下任一参数的有效值。

| 参数 | 类型   | 说明                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | 指定在多长时间内聚合报表。 受支持的 {period_value} 值为：D7、D30、D90 和 D180。 这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。 |
| date      | Date   | 指定要查看用户在哪个日期执行的任何活动。 {date_value} 必须采用格式 YYYY-MM-DD。 因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。 |

> **注意：** 需要在 URL 中设置 period 或 date。

此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。 默认输出类型为 text/csv。 但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## <a name="response"></a>响应

### <a name="csv"></a>CSV

如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。 可以在响应的 `Location` 头中找到此 URL。

预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。

CSV 文件包含下面的列标题。

- 报表刷新日期
- 网站 URL
- 所有者显示名称
- 已删除
- 上次活动日期
- 文件数
- 活跃文件数
- 已使用的存储（字节）
- 已分配的存储（字节）
- 所有者主体名称
- 报表周期

### <a name="json"></a>JSON

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和**[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** 对象。

此请求的默认页面大小为200个项目。

## <a name="example"></a>示例

下面是输出 CSV 的示例。

### <a name="csv"></a>CSV

#### <a name="request"></a>请求

下面展示了示例请求。


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a>响应

下面展示了示例响应。

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

执行 302 重定向，下载的 CSV 文件将采用以下架构。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Owner Principal Name,Report Period
```

### <a name="json"></a>JSON

下面是一个返回 JSON 的示例。

#### <a name="request"></a>请求

下面展示了示例请求。


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```


#### <a name="response"></a>响应

下面展示了示例响应。

> **Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 9, 
      "activeFileCount": 5, 
      "storageUsedInBytes": 12190375, 
      "storageAllocatedInBytes": 549755813880, 
      "reportPeriod": "7"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

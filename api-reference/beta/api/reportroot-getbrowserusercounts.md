---
title: reportRoot： getBrowserUserCounts
description: 获取一个报告，该报告提供在选定时段内使用 Microsoft Edge、Microsoft Edge 旧版 和 Internet Explorer 访问 Microsoft 365 服务的活动用户数趋势。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 256d26b58be2e08f3fde1bb772aeb7c09656e929
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589605"
---
# <a name="reportroot-getbrowserusercounts"></a>reportRoot： getBrowserUserCounts

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取一个报告，该报告提供在选定时段内使用 Microsoft Edge、Microsoft Edge 旧版 和 Internet Explorer 访问 Microsoft 365 服务的活动用户数趋势。

> **注意：** 有关不同报告视图和名称的详细信息，请参阅Microsoft 365中心 [的报告 - Microsoft 浏览器使用情况](/microsoft-365/admin/activity-reports/browser-usage-report)。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| -------------------------------------- | -------------------------------------------- |
| 委派（工作或学校帐户）     | Reports.Read.All                            |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用                            | Reports.Read.All                            |

> **注意：** 对于允许应用代表用户读取服务使用情况报表的委派权限，租户管理员必须为用户分配适当的Azure Active Directory有限管理员角色。 有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getBrowserUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a>函数参数

在请求 URL 中，提供以下参数的有效值。

| 参数 | 类型   | 说明                                                                                                                                                                                                                                                       |
| --------- | ------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| period    | string | 指定在多长时间内聚合报表。 {period_value} 支持的值是：、`D7`、`D30`和 `D90``D180`。 这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。 必需。 |

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。 默认输出类型为 `text/csv`。 但是，如果要指定输出类型，可以使用 OData `$format` 查询参数将默认输出 `text/csv` 设置为 或 `application/json`。

## <a name="request-headers"></a>请求头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

### <a name="csv"></a>CSV

如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。 可以在响应的 `Location` 头中找到此 URL。

预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。

CSV 文件包含下面的列标题：

- 报表刷新日期
- 报表周期
- 报表日期
- Microsoft Edge
- 旧版边缘
- Internet Explorer

### <a name="json"></a>JSON

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 JSON 对象。

## <a name="examples"></a>示例

### <a name="example-1-csv-output"></a>示例 1：CSV 输出

下面是输出 CSV 的示例。

#### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getbrowserusercounts_csv"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getBrowserUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- { "blockType": "response" } -->
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

Report Refresh Date, Report Period, Report Date, Edge, Edge Legacy, Internet Explorer
```

### <a name="example-2-json-output"></a>示例 2：JSON 输出

下面是返回 JSON 的示例。

#### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getbrowserusercounts_json"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getBrowserUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 205

{
   "value":[
      {
         "reportRefreshDate":"2021-04-17",
         "reportPeriod":7,
         "userCounts":[
            {
               "reportDate":"2021-04-17",
               "edge":413,
               "edgeLegacy":11,
               "ie":21
            },
            {
               "reportDate":"2021-04-16",
               "edge":883,
               "edgeLegacy":26,
               "ie":124
            }
         ]
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

---
title: 'reportRoot: getSharePointSiteUsageFileCounts'
description: 获取跨所有网站的文件总数和活跃文件数。 如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 540ce54eb69ff21641f017e6db46a288bbfd8d3e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897664"
---
# <a name="reportroot-getsharepointsiteusagefilecounts"></a>reportRoot: getSharePointSiteUsageFileCounts

命名空间：microsoft.graph

获取跨所有网站的文件总数和活跃文件数。 如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 报表-SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。

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
GET /reports/getSharePointSiteUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a>函数参数

在请求 URL 中，提供以下参数的有效值。

| 参数 | 类型   | 说明                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | 指定在多长时间内聚合报表。 受支持的 {period_value} 值为：D7、D30、D90 和 D180。 这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。 必需。 |

## <a name="request-headers"></a>请求标头

| 名称          | 说明                              |
| :------------ | :--------------------------------------- |
| Authorization | Bearer {token}. Required.                |
| If-None-Match | 如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。 可选。 |

## <a name="response"></a>响应

如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。 可以在响应的 `Location` 头中找到此 URL。

预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。

CSV 文件包含下面的列标题。

- 报表刷新日期
- 网站类型
- 总计
- 活跃
- 报表日期
- 报表周期

## <a name="example"></a>示例

#### <a name="request"></a>请求

下面展示了示例请求。


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagefilecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageFileCounts(period='D7')
```


#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

执行 302 重定向，下载的 CSV 文件将采用以下架构。

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
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

---
title: reportRoot： getTeamsTeamActivityDistributionCounts
description: 获取所选时间段内跨Microsoft Teams的团队活动数。
ms.localizationpriority: medium
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9abf55803b2bbbdf2d70d0fcde78ef5fff2e4987
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917844"
---
# <a name="reportroot-getteamsteamactivitydistributioncounts"></a>reportRoot： getTeamsTeamActivityDistributionCounts

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取所选时间段内跨Microsoft Teams的团队活动数。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :--------------------------------------- |
| 委派（工作或学校帐户）     | Reports.Read.All                         |
| 委派（个人 Microsoft 帐户） | 不支持。                           |
| 应用                            | Reports.Read.All                         |

> **注意：** 对于允许应用代表用户读取服务使用情况报告的委派权限，租户管理员必须为用户分配适当的Azure Active Directory受限管理员角色。 有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsTeamActivityDistributionCounts(period='{period_value}')
```

## <a name="function-parameters"></a>函数参数

在请求 URL 中，提供以下参数的有效值。

| 参数 | 类型   | 说明                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | 指定在多长时间内聚合报表。 {period_value} 支持的值为： `D7`、 和 `D90``D30``D180`. 这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。 必需。 |

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。 默认输出类型为 `text/csv`. 但是，如果要指定输出类型，可以使用 OData `$format` 查询参数将默认输出设置为 `text/csv` 或 `application/json`设置。

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="response"></a>响应

### <a name="csv"></a>CSV

如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。 可以在响应的 `Location` 头中找到此 URL。

预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。

CSV 文件包含下面的列标题：

- 报表刷新日期
- 报表周期
- 活动用户
- 活动通道
- 来宾
- 反应
- 组织会议
- 发布消息
- 频道消息
- 活动共享通道
- 活动外部用户
- 回复消息
- 紧急消息
- 提及

### <a name="json"></a>JSON

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 JSON 对象。

## <a name="examples"></a>示例

### <a name="example-1-csv-output"></a>示例 1：CSV 输出

下面是输出 CSV 的示例。

#### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsteamactivitydistributioncounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsTeamActivityDistributionCounts(period='D7')?$format=text/csv
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

Report Refresh Date,Report Period,Active Users,Active Channels,Guests,Reactions,Meetings Organized,Post Messages,Channel Messages,Active Shared Channels,Active External Users,Reply Messages,Urgent Messages,Mentions
```

### <a name="example-2-json-output"></a>示例 2：JSON 输出

下面是返回 JSON 的示例。

#### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsteamactivitydistributioncounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsTeamActivityDistributionCounts(period='D7')?$format=application/json
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
Content-Length: 575

{
  "@odata.context": "https://graph.microsoft.com/beta/reports/getTeamsTeamActivityDistributionCounts(period='D7')?$format=application/json&$skiptoken=D07uj", 
  "value": [
    {
      "reportRefreshDate": "2021-09-01", 
      "userCounts": [
        "reportPeriod":7,
        "activeUsers": 26, 
        "activeChannels": 17, 
        "guests": 4, 
        "reactions": 36, 
        "meetingsOrganized": 0,
        "postMessages": 83,
        "channelMessages": 101,
        "activeSharedChannels": 1,
        "activeExternalUsers": 2,
        "replyMessages":10,
        "urgentMessages":8,
        "mentions":1
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

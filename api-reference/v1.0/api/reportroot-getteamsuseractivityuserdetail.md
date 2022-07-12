---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: 按用户获取有关 Microsoft Teams 用户活动的详细信息。
ms.localizationpriority: high
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 934206863b13e5e7e3a1a5918f6fc630561fa470
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730383"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a>reportRoot: getTeamsUserActivityUserDetail

命名空间：microsoft.graph

按用户获取有关 Microsoft Teams 用户活动的详细信息。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :--------------------------------------- |
| 委派（工作或学校帐户）     | Reports.Read.All                         |
| 委派（个人 Microsoft 帐户） | 不支持。                           |
| 应用                            | Reports.Read.All                         |

>**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。有关更多详细信息，请参阅 [ API 授权，读取 Microsoft 365使用情况报告](/graph/reportroot-authorization)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a>函数参数

在请求 URL 中，提供以下任一参数的有效值。

| 参数 | 类型   | 说明                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | 指定在多长时间内聚合报表。 受支持的 {period_value} 值为：D7、D30、D90 和 D180。 这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。 |
| date      | Date   | 指定要查看用户在哪个日期执行的任何活动。 {date_value} 必须采用格式 YYYY-MM-DD。 因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。 |

> **注意：** 需要在 URL 中设置 period 或 date。

## <a name="request-headers"></a>请求头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。 可以在响应的 `Location` 头中找到此 URL。

预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。

CSV 文件包含下面的列标题：

- 报表刷新日期
- 租户显示名称
- 共享频道租户显示名称
- User Id
- 用户主体名称
- 上次活动日期
- 已删除
- 删除日期
- 分配的产品
- 团队聊天消息计数
- 专用聊天消息计数
- 呼叫计数
- 会议计数
- 发布消息
- 回复消息
- 紧急消息
- 组织会议数量
- 参加会议数量
- 临时组织会议数量
- 临时出席会议数量
- 安排组织的一次性会议数量
- 安排出席的一次性会议数量
- 安排组织的定期会议数量
- 安排出席的定期会议数量
- 音频持续时间
- 视频持续时间
- 屏幕共享持续时间
- 音频持续时间（以秒为单位）
- 视频持续时间（以秒为单位）
- 屏幕共享持续时间（以秒为单位）
- 包含其他操作
- 已获得许可
- 报表周期

> [!NOTE] 
> “组织会议数量”中的值可能不是用户在指定时间段内组织的“临时组织会议数量”、“安排组织的一次性会议数量”和“安排组织的定期会议数量”的总和。 这是因为输出 CSV 文件中未包含未分类的会议值。 有关详细信息，请参阅 [Microsoft Teams 用户活动报告](https://docs.microsoft.com/microsoftteams/teams-analytics-and-reports/user-activity-report)。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```


### <a name="response"></a>响应

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

Report Refresh Date,Tenant Display Name,Shared Channel Tenant Display Names,User Id,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Post Messages,Reply Messages,Urgent Messages,Meetings Organized Count,Meetings Attended Count,Ad Hoc Meetings Organized Count,Ad Hoc Meetings Attended Count,Scheduled One-time Meetings Organized Count,Scheduled One-time Meetings Attended Count,Scheduled Recurring Meetings Organized Count,Scheduled Recurring Meetings Attended Count,Audio Duration,Video Duration,Screen Share Duration,Audio Duration In Seconds,Video Duration In Seconds,Screen Share Duration In Seconds,Has Other Action,Is Licensed,Report Period
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


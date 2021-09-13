---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: 按活动类型获取 Microsoft Teams 用户的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 7618c2026ae3a272c1c7ff4cc59bc3e54d0ae3df
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59050045"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a>reportRoot: getTeamsUserActivityUserCounts

命名空间：microsoft.graph

按活动类型获取 Microsoft Teams 用户的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :--------------------------------------- |
| 委派（工作或学校帐户）     | Reports.Read.All                         |
| 委派（个人 Microsoft 帐户） | 不支持。                           |
| 应用                            | Reports.Read.All                         |

**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。有关更多详细信息，请参阅 [ API 授权，读取 Microsoft 365使用情况报告](/graph/reportroot-authorization)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a>函数参数

在请求 URL 中，提供以下参数的有效值。

| 参数 | 类型   | 说明                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | 指定在多长时间内聚合报表。 受支持的 {period_value} 值为：D7、D30、D90 和 D180。 这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。 必需。 |

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="response"></a>响应

如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。 可以在响应的 `Location` 头中找到此 URL。

预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。

CSV 文件包含下面的列标题：

- 报表刷新日期
- 报表日期
- 团队聊天消息
- 专用聊天消息
- 呼叫
- 会议
- 其他操作
- 报表周期

## <a name="example"></a>示例

#### <a name="request"></a>请求

下面展示了示例请求。


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
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

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
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


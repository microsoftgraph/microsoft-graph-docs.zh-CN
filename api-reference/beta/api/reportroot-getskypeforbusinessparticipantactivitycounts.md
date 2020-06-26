---
title: 'reportRoot: getSkypeForBusinessParticipantActivityCounts'
description: 获取使用情况趋势，即组织中用户参与的会议会话的次数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 801d516bdefaeaa1b8fb6e9ed357add27ff301a1
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896663"
---
# <a name="reportroot-getskypeforbusinessparticipantactivitycounts"></a>reportRoot: getSkypeForBusinessParticipantActivityCounts

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取使用情况趋势，即组织中用户参与的会议会话的次数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 reports-Skype For business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。

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
GET /reports/getSkypeForBusinessParticipantActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a>函数参数

在请求 URL 中，提供以下参数的有效值。

| 参数 | 类型   | 说明                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | 指定在多长时间内聚合报表。 受支持的 {period_value} 值为：D7、D30、D90 和 D180。 这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。 必需。 |

此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。 默认输出类型为 text/csv。 但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。

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
- 报表日期
- 报表周期
- IM
- 音频/视频
- 应用共享
- Web
- 第三方拨入/拨出

### <a name="json"></a>JSON

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和**[skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md)** 对象。

## <a name="example"></a>示例

### <a name="csv"></a>CSV

下面是输出 CSV 的示例。

#### <a name="request"></a>请求

下面展示了示例请求。


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')?$format=text/csv
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

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```

### <a name="json"></a>JSON

下面是一个返回 JSON 的示例。

#### <a name="request"></a>请求

下面展示了示例请求。


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')?$format=application/json
```


#### <a name="response"></a>响应

下面展示了示例响应。

> **Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 296

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityCounts)", 
  "value": [
    {
      "im": 162, 
      "audioVideo": 156, 
      "appSharing": 45, 
      "web": 12, 
      "dialInOut3rdParty": 2, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
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

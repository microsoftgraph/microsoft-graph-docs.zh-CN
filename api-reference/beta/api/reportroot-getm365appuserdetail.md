---
title: reportRoot： getM365AppUserDetail
description: 获取提供有关用户已使用的应用程序和平台的详细信息的报告。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 924a3135af954d6c0fda57b7b50a4022a8dffef6
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630404"
---
# <a name="reportroot-getm365appuserdetail"></a>reportRoot： getM365AppUserDetail

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取提供有关用户已使用的应用程序和平台的详细信息的报告。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅[microsoft 365 报表-microsoft 365 应用程序使用](https://docs.microsoft.com/microsoft-365/admin/activity-reports/microsoft365-apps-usage)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | Reports.Read.All                            |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用                            | Reports.Read.All                            |

> **注意：** 为使应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。 有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getM365AppUserDetail(period='{period_value}')
GET /reports/getM365AppUserDetail(date={date_value})
```

## <a name="function-parameters"></a>函数参数

在请求 URL 中，提供以下参数的有效值。

| 参数 | 类型   | 说明                                                                                                                                                                                                                                             |
| :-------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| period    | string | 指定在多长时间内聚合报表。 {Period_value} 支持的值为： `D7` 、 `D30` 、 `D90` 、和 `D180` 。 这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。 |
| date      | Date   | 指定要查看用户在哪个日期执行的任何活动。 {date_value} 必须采用格式 YYYY-MM-DD。 因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。          |

> **注意：** 您需要 `period` `date` 在 URL 中设置或。

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。 默认输出类型为 text/csv。 但是，如果要指定输出类型，则可以使用 OData `$format` 查询参数将默认输出设置为 text/csv 或 application/json。

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿为此方法提供请求正文。

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[report](../resources/intune-shared-report.md)对象。 报告数据包含在**report**对象的**content**属性中。

### <a name="csv"></a>CSV

如果成功，请求**content**属性将返回一个 `302 Found` 响应，该响应将重定向到报告的 preauthenticated 下载 URL。 可以在响应的 `Location` 头中找到此 URL。

预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。

CSV 文件包含下面的列标题：

- 报表刷新日期
- 用户主体名称
- 上次激活日期
- 上次活动日期
- 报表周期
- Windows
- Mac
- 移动
- Web
- Outlook
- Word
- Excel
- PowerPoint
- OneNote
- Teams
- Outlook (Windows) 
- Word (Windows) 
- Excel (Windows) 
- PowerPoint (Windows) 
- OneNote (Windows) 
- 团队 (Windows) 
- Outlook (Mac) 
- Word (Mac) 
- Excel (Mac) 
- PowerPoint (Mac) 
- OneNote (Mac) 
-  (Mac) 的团队
- Outlook (移动) 
- Word (移动) 
- Excel (移动) 
- PowerPoint (移动) 
- OneNote (移动) 
-  (移动) 的团队
- Outlook (Web) 
- Word (Web) 
- Excel (Web) 
- PowerPoint (Web) 
- OneNote (Web) 
-  (Web) 的团队

### <a name="json"></a>JSON

如果成功，请求**content**属性将 `200 OK` 在响应正文中返回响应代码和 JSON 对象。

此请求的默认页面大小为200个项目。

## <a name="examples"></a>示例

### <a name="example-1-csv-output"></a>示例1： CSV 输出

下面是输出 CSV 的示例。

#### <a name="request"></a>请求

下面的示例显示了获取**内容**属性的请求。


<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCounDetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=text/csv
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

Report Refresh Date,User Principal Name,Last Activation Date,Last Activity Date,Report Period,Windows,Mac,Mobile,Web,Outlook,Word,Excel,PowerPoint,OneNote,Teams,Outlook (Windows),Word (Windows),Excel (Windows),PowerPoint (Windows),OneNote (Windows),Teams (Windows),Outlook (Mac),Word (Mac),Excel (Mac),PowerPoint (Mac),OneNote (Mac),Teams (Mac),Outlook (Mobile),Word (Mobile),Excel (Mobile),PowerPoint (Mobile),OneNote (Mobile),Teams (Mobile),Outlook (Web),Word (Web),Excel (Web),PowerPoint (Web),OneNote (Web),Teams (Web)
```

### <a name="example-2-json-output"></a>示例2： JSON 输出

下面是一个返回 JSON 的示例。

#### <a name="request"></a>请求

下面的示例显示了获取**内容**属性的请求。


<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCountDetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=application/json
```


#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 951

{
  "@odata.nextLink": "https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=application/json&$skiptoken=AAAAA",
  "value": [
    {
      "reportRefreshDate": "2020-06-30",
      "userPrincipalName": "admin@contoso.com",
      "lastActivationDate": "2020-05-22",
      "lastActivityDate": "2020-06-30",
      "details": [
        {
          "reportPeriod": 7,
          "windows": true,
          "mac": false,
          "mobile": true,
          "web": false,
          "outlook": false,
          "word": false,
          "excel": false,
          "powerPoint": false,
          "oneNote": false,
          "teams": true,
          "outlookWindows": false,
          "wordWindows": false,
          "excelWindows": false,
          "powerPointWindows": false,
          "oneNoteWindows": false,
          "teamsWindows": true,
          "outlookMac": false,
          "wordMac": false,
          "excelMac": false,
          "powerPointMac": false,
          "oneNoteMac": false,
          "teamsMac": false,
          "outlookMobile": false,
          "wordMobile": false,
          "excelMobile": false,
          "powerPointMobile": false,
          "oneNoteMobile": false,
          "teamsMobile": true,
          "outlookWeb": false,
          "wordWeb": false,
          "excelWeb": false,
          "powerPointWeb": false,
          "oneNoteWeb": false,
          "teamsWeb": true
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

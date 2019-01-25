---
title: 获取 educationSynchronizationProfile 的状态
description: 为租户中获取特定学校数据同步配置文件的状态。 响应将指示的同步的状态。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6a2d3dffd715d78bb96794808da39255db0164b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510195"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a>获取 educationSynchronizationProfile 的状态

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取租户中的特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的状态。 响应将指示的同步的状态。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:-----------|:----------|
| 委派（工作或学校帐户） | EduAdministration.Read EduAdministration.ReadWrite |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| EduAdministration.Read.All EduAdministration.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md)对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a>响应
下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2017-07-04T22:06:37.6472621Z"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofilestatus-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

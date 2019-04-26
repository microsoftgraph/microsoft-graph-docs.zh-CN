---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: 获取分析结果
localization_priority: Normal
ms.openlocfilehash: fb8986351aec3afb88a4c6034a52781423e543f0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338779"
---
# <a name="get-analytics"></a>获取分析结果

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取有关在此资源下发生的视图的[itemAnalytics][] 。
**itemAnalytics**资源是获取`allTime`和的`lastSevenDays`活动统计信息的便捷方式。
对于自定义时间范围或时间间隔, 请使用[getActivitiesByInterval][] API。

>**注意:****itemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）
|:--------------------------------------|:-------------------------------------
|委派（工作或学校帐户）     | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All
|委派（个人 Microsoft 帐户） | 不支持。
|应用程序                            | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a>示例

#### <a name="request"></a>请求

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a>响应

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "allTime": {
        "access": {
            "actionCount": 123,
            "actorCount": 89
        }
    },
    "lastSevenDays": {
        "access": {
            "actionCount": 52,
            "actorCount": 41
        }
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": []
}
-->

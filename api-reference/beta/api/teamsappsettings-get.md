---
title: 获取 teamsAppSettings
description: 读取 teamsAppSettings 对象的属性和关系。
author: subray2014
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bd04f3dcdb72775ec372763cb12e94ccbead9a0d
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645618"
---
# <a name="get-teamsappsettings"></a>获取 teamsAppSettings
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [teamsAppSettings 对象的](../resources/teamsappsettings.md) 属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|TeamworkAppSettings.Read.All、TeamworkAppSettings.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|Application|不支持|

> [!NOTE]
> TeamworkAppSettings.* 权限可能在Azure 门户中不可见。 有关详细信息和解决方法，请参阅 [已知问题](/graph/known-issues#teamworkappsettings-permissions-are-not-visible-in-the-azure-portal)。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/teamsAppSettings
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [teamsAppSettings](../resources/teamsappsettings.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-get-the-tenant-wide-settings-for-all-teams-apps-in-the-tenant"></a>示例 1：获取租户中所有 Teams 应用的租户范围设置。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_teamsappsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/teamsAppSettings
```


#### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamsAppSettings",
    "id": "65bdf003-0c4c-4bca-b102-0821ab0d1364",
    "isChatResourceSpecificConsentEnabled": "true"
  }
}
```

## <a name="see-also"></a>另请参阅

- [特定于资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)
---
title: 更新 teamsAppSettings
description: 更新 teamsAppSettings 对象的属性。
author: subray2014
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5fdcc9fafe199e11881c59e65842c09d955eb74e
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645632"
---
# <a name="update-teamsappsettings"></a>更新 teamsAppSettings
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [teamsAppSettings 对象的](../resources/teamsappsettings.md) 属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

>**注意：** 只有全局管理员和 Teams 管理员才能调用此 API。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|TeamworkAppSettings.ReadWrite.All|
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
PATCH /teamwork/teamsAppSettings
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|属性|类型|说明|
|:---|:---|:---|
|isChatResourceSpecificConsentEnabled|Boolean|指示是否已为租户启用特定于资源的聊天/会议许可。 如果为 true，则可以在聊天和会议中安装允许在租户中且需要资源特定权限的 Teams 应用。 如果为 false，则会阻止在聊天或会议中安装需要资源特定权限的任何 Teams 应用。|



## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-enable-installation-of-apps-that-require-resource-specific-consent-in-chatsmeetings"></a>示例 1：在聊天/会议中启用需要资源特定许可的应用的安装。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "update_teamsappsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teamwork/teamsAppSettings
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamsAppSettings",
  "isChatResourceSpecificConsentEnabled": "true"
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>另请参阅

- [特定于资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)
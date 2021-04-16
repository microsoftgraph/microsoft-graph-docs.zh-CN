---
title: 更新 windowsQualityUpdateCatalogItem
description: 更新 windowsQualityUpdateCatalogItem 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5dcaadfea931ef5d6e9a1fce5bc9e948269d390b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868035"
---
# <a name="update-windowsqualityupdatecatalogitem"></a>更新 windowsQualityUpdateCatalogItem

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [windowsQualityUpdateCatalogItem 对象](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) 对象的 JSON 表示形式。

下表显示创建 [windowsQualityUpdateCatalogItem 时所需的属性](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|目录项 ID。继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|displayName|String|目录显示名称列表。 继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|releaseDateTime|DateTimeOffset|目录项的发布日期 继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|endOfSupportDate|DateTimeOffset|目录项的上次支持日期 继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|kbArticleId|String|知识库文章 ID|
|classification|[windowsQualityUpdateClassification](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|质量更新的分类。 可取值为：`all`、`security`、`nonSecurity`。|
|isExpeditable|Boolean|指示更新是否符合加速条件的标志|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
Content-type: application/json
Content-length: 332

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
  "kbArticleId": "Kb Article Id value",
  "classification": "security",
  "isExpeditable": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 381

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "id": "8eb831ba-31ba-8eb8-ba31-b88eba31b88e",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
  "kbArticleId": "Kb Article Id value",
  "classification": "security",
  "isExpeditable": true
}
```





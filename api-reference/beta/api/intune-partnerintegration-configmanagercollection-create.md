---
title: 创建 configManagerCollection
description: 创建新的 configManagerCollection 对象。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 945a4bedf5a0680b001307a0d829cebc606c6812
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59070018"
---
# <a name="create-configmanagercollection"></a>创建 configManagerCollection

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configManagerCollections
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 configManagerCollection 对象的 JSON 表示形式。

下表显示创建 configManagerCollection 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|ConfigManager 集合的键。|
|displayName|String|DisplayName。|
|collectionIdentifier|String|SCCM 中的集合标识符。|
|hierarchyName|String|HierarchyName。|
|hierarchyIdentifier|String|层次结构标识符。|
|createdDateTime|DateTimeOffset|创建日期。|
|lastModifiedDateTime|DateTimeOffset|上次修改日期。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configManagerCollections
Content-type: application/json
Content-length: 263

{
  "@odata.type": "#microsoft.graph.configManagerCollection",
  "displayName": "Display Name value",
  "collectionIdentifier": "Collection Identifier value",
  "hierarchyName": "Hierarchy Name value",
  "hierarchyIdentifier": "Hierarchy Identifier value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 435

{
  "@odata.type": "#microsoft.graph.configManagerCollection",
  "id": "5f9d1d76-1d76-5f9d-761d-9d5f761d9d5f",
  "displayName": "Display Name value",
  "collectionIdentifier": "Collection Identifier value",
  "hierarchyName": "Hierarchy Name value",
  "hierarchyIdentifier": "Hierarchy Identifier value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




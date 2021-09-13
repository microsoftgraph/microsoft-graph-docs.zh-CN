---
title: 创建 groupPolicyObjectFile
description: 创建新的 groupPolicyObjectFile 对象。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f61b8459b716673dde30bcea4aacabd6286c8801
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59121709"
---
# <a name="create-grouppolicyobjectfile"></a>创建 groupPolicyObjectFile

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) 对象。

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
POST /deviceManagement/groupPolicyObjectFiles
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 groupPolicyObjectFile 对象的 JSON 表示形式。

下表显示创建 groupPolicyObjectFile 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|groupPolicyObjectId|Guid|来自 GPO Xml 内容的组策略对象 GUID|
|ouDistinguishedName|String|OU 的可分辨名称。|
|createdDateTime|DateTimeOffset|首次上载 GroupPolicy 的日期和时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改 GroupPolicyObjectFile 的日期和时间。|
|内容|String|组策略对象文件内容。|



## <a name="response"></a>响应
如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyObjectFiles
Content-type: application/json
Content-length: 217

{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "content": "Content value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 389

{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "id": "65c0499d-499d-65c0-9d49-c0659d49c065",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "content": "Content value"
}
```




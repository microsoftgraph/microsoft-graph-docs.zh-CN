---
title: 创建 groupPolicyUploadedDefinitionFile
description: 创建新的 groupPolicyUploadedDefinitionFile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0de13716e978eb74d96d45a66a46a571680a0f8f9d8e1c05cf733dcc8a7243bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145738"
---
# <a name="create-grouppolicyuploadeddefinitionfile"></a>创建 groupPolicyUploadedDefinitionFile

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) 对象。

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
POST /deviceManagement/groupPolicyUploadedDefinitionFiles
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 groupPolicyUploadedDefinitionFile 对象的 JSON 表示形式。

下表显示创建 groupPolicyUploadedDefinitionFile 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|ADMX 文件的本地化友好名称。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|description|String|ADMX 文件中策略设置的本地化说明。 默认值为空白。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|languageCodes|String collection|ADMX 文件支持的语言代码。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|targetPrefix|String|指定引用 ADMX 文件内的命名空间的逻辑名称。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|targetNamespace|String|指定用于标识 ADMX 文件内的命名空间的 URI。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|指定组策略的类型。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)。 可取值为：`admxBacked`、`admxIngested`。|
|revision|String|与文件关联的修订版本。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|id|字符串|实体的键。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|fileName|String|已上载的 ADML 文件的文件名。|
|status|[groupPolicyUploadedDefinitionFileStatus](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfilestatus.md)|已上载的 ADMX 文件的上载状态。 可取值为：`none`、`uploadInProgress`、`available`、`assigned`、`removalInProgress`、`uploadFailed` 或 `removalFailed`。|
|content|二进制|上载的 ADMX 文件的内容。|
|uploadDateTime|DateTimeOffset|上传的 ADMX 文件的上传时间。|
|defaultLanguageCode|字符串|上载的 ADMX 文件的默认语言。|
|groupPolicyUploadedLanguageFiles|[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) 集合|与上载的 ADMX 文件关联的 ADML 文件列表。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles
Content-type: application/json
Content-length: 922

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "fileName": "File Name value",
  "status": "uploadInProgress",
  "content": "Y29udGVudA==",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00",
  "defaultLanguageCode": "Default Language Code value",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "File Name value",
      "languageCode": "Language Code value",
      "content": "Y29udGVudA==",
      "id": "Id value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1035

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "id": "0ce1a8cf-a8cf-0ce1-cfa8-e10ccfa8e10c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "fileName": "File Name value",
  "status": "uploadInProgress",
  "content": "Y29udGVudA==",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00",
  "defaultLanguageCode": "Default Language Code value",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "File Name value",
      "languageCode": "Language Code value",
      "content": "Y29udGVudA==",
      "id": "Id value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```





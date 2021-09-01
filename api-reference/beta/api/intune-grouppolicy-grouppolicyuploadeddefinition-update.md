---
title: 更新 groupPolicyUploadedDefinition
description: 更新 groupPolicyUploadedDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 39960405902cb10db7decc6392aabd012d1025c9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819926"
---
# <a name="update-grouppolicyuploadeddefinition"></a>更新 groupPolicyUploadedDefinition

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [groupPolicyUploadedDefinition 对象](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 的属性。

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
PATCH /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/nextVersionDefinition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/previousVersionDefinition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/{groupPolicyDefinitionId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [groupPolicyUploadedDefinition 对象的](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) JSON 表示形式。

下表显示创建 [groupPolicyUploadedDefinition 时所需的属性](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)。

|属性|类型|Description|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|标识策略可应用于的组类型。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。 可取值为：`user`、`machine`。|
|displayName|字符串|本地化的策略名称。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|explainText|字符串|与策略关联的本地化说明或帮助文本。 默认值为空白。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|categoryPath|字符串|策略的本地化完整类别路径。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|supportedOn|字符串|用于指定受策略影响的操作系统或应用程序版本的本地化字符串。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|指定组策略的类型。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。 可取值为：`admxBacked`、`admxIngested`。|
|hasRelatedDefinitions|Boolean|表示此定义是否有相关定义 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|groupPolicyCategoryId|Guid|父类别的类别 ID 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|minDeviceCspVersion|String|此定义中设备配置所需的最低 CSP 版本 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|minUserCspVersion|String|此定义中用户配置所需的最低 CSP 版本 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|version|String|设置定义版本 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|id|字符串|实体的键。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 538

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "hasRelatedDefinitions": true,
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
  "minDeviceCspVersion": "Min Device Csp Version value",
  "minUserCspVersion": "Min User Csp Version value",
  "version": "Version value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "hasRelatedDefinitions": true,
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
  "minDeviceCspVersion": "Min Device Csp Version value",
  "minUserCspVersion": "Min User Csp Version value",
  "version": "Version value",
  "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




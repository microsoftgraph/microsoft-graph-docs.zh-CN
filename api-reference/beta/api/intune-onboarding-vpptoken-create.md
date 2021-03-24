---
title: 创建 vppToken
description: 创建新的 vppToken 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 035e7917be4ba7fea7470f03bd5e3273cbdc8776
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135010"
---
# <a name="create-vpptoken"></a>创建 vppToken

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 vppToken 对象的 JSON 表示形式。

下表显示创建 vppToken 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|这是创建 appleVolumePurchaseProgramToken 时自动生成的。 它是实体的键。|
|organizationName|String|与 Apple Volume Purchase Program 令牌关联的组织|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。 可取值为：`business`、`education`。 可取值为：`business`、`education`。|
|appleId|String|与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。|
|expirationDateTime|DateTimeOffset|Apple Volume Purchase Program 令牌的到期日期时间。|
|lastSyncDateTime|DateTimeOffset|上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。|
|token|String|从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。|
|lastModifiedDateTime|DateTimeOffset|与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。|
|state|[vppTokenState](../resources/intune-onboarding-vpptokenstate.md)|Apple Volume Purchase Program 令牌的当前状态。 可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。 可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`、`duplicateLocationId`。|
|tokenActionResults|[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) 集合|对 Apple Volume Purchase Program 令牌执行的操作的状态集合。|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune-onboarding-vpptokensyncstatus.md)|使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。 可取值为：`none`、`inProgress`、`completed`、`failed`。 可取值为：`none`、`inProgress`、`completed`、`failed`。|
|automaticallyUpdateApps|Boolean|是否自动更新适用于 VPP 令牌的应用。|
|countryOrRegion|String|是否自动更新适用于 VPP 令牌的应用。|
|dataSharingConsentGranted|Boolean|同意与 Apple Volume Purchase Program 共享数据。|
|displayName|String|管理员指定的令牌友好名称。|
|locationName|String|从 Apple VPP 返回的令牌位置。|
|claimTokenManagementFromExternalMdm|Boolean|管理员同意允许从外部 MDM 进行声明令牌管理。|
|roleScopeTagIds|String collection|角色作用域标记分配给此实体的标识。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
Content-type: application/json
Content-length: 1002

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1115

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





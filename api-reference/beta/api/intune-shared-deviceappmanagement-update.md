---
title: 更新 deviceAppManagement
description: 更新 deviceAppManagement 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cb9e1864c48cf652f2a59dd3146c0f28eb05312c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868143"
---
# <a name="update-deviceappmanagement"></a>更新 deviceAppManagement

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性。
## <a name="prerequisites"></a>先决条件
以下权限之一需要调用此 API。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。  请注意，在相应权限根据工作流而有所不同。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
| 委派（工作或学校帐户） | |
| &nbsp;&nbsp; **应用程序**、**书籍**或**入职培训** | DeviceManagementApps.ReadWrite.All |
| &nbsp; &nbsp; **设备管理** | DeviceManagementManagedDevices.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的 JSON 表示形式。

下表显示创建 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|**在白板**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。|
|microsoftStoreForBusinessLanguage|String|用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。 特定于国家/地区的区域性。 这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。 格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。 例如，“en-US”（“英语(美国)）是一个特定的区域性。|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|从适用于企业的 Microsoft Store 的应用程序同步上次完成的时间。|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。|
|microsoftStoreForBusinessPortalSelection|[microsoftStoreForBusinessPortalSelectionOptions](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|最终用户门户信息用于同步 Intune 的公司门户从 Microsoft 存储的业务应用程序。 有三个选项，可以从中进行选取\[公司仅门户、 公司门户和专用存储、 仅专用存储\]。 可取值为：`none`、`companyPortal`、`privateStore`。|

此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。

## <a name="response"></a>响应
如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a>响应

下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```




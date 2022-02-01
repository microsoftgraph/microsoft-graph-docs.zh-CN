---
title: 创建 oemWarrantyInformationOnboarding
description: 创建新的 oemWarrantyInformationOnboarding 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 710fb48056c8527a82f5202e1b0910e1c8312444
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292283"
---
# <a name="create-oemwarrantyinformationonboarding"></a>创建 oemWarrantyInformationOnboarding

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/oemWarrantyInformationOnboarding
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 oemWarrantyInformationOnboarding 对象的 JSON 表示形式。

下表显示创建 oemWarrantyInformationOnboarding 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|OEM 担保状态的唯一标识符。 此属性是只读的。|
|oemName|String|OEM 名称。 此属性是只读的。|
|enabled|Boolean|指定是否对给定的 OEM 启用担保查询。 此属性是只读的。|
|可用|Boolean|指定是否提供担保 API。 此属性是只读的。|



## <a name="response"></a>响应
如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/oemWarrantyInformationOnboarding
Content-type: application/json
Content-length: 148

{
  "@odata.type": "#microsoft.graph.oemWarrantyInformationOnboarding",
  "oemName": "Oem Name value",
  "enabled": true,
  "available": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 197

{
  "@odata.type": "#microsoft.graph.oemWarrantyInformationOnboarding",
  "id": "55491425-1425-5549-2514-495525144955",
  "oemName": "Oem Name value",
  "enabled": true,
  "available": true
}
```





---
title: azureADDeviceRegistrationError 资源类型
description: 在设备注册过程中Azure AD，该错误阻止服务在更新管理中注册设备或将内容部署到设备。
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 8ef1d16203f4b2197a0f8cdb93aaeae073d77ccb
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890365"
---
# <a name="azureaddeviceregistrationerror-resource-type"></a>azureADDeviceRegistrationError 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在设备注册过程中[Azure AD，](../resources/windowsupdates-azureaddevice.md)该错误阻止服务在更新管理中注册设备或将内容部署到设备。

继承自 [updatableAssetError](../resources/windowsupdates-updatableasseterror.md)。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|reason|microsoft.graph.windowsUpdates.azureADDeviceRegistrationErrorReason|注册遇到错误的原因。 可取值为：`invalidGlobalDeviceId`、`invalidAzureADDeviceId`、`missingTrustType`、`invalidAzureADJoin`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.azureADDeviceRegistrationError",
  "reason": "String"
}
```


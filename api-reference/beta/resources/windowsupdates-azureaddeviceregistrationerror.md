---
title: azureADDeviceRegistrationError 资源类型
description: Azure AD 设备的注册过程中出现一个错误，该错误阻止该服务在更新管理中注册设备或将内容部署到设备。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 1d08ab96d5298c70f34acf89e3c6c4605d9df0a1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067862"
---
# <a name="azureaddeviceregistrationerror-resource-type"></a>azureADDeviceRegistrationError 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure [AD](../resources/windowsupdates-azureaddevice.md) 设备的注册过程中出现一个错误，该错误阻止该服务在更新管理中注册设备或将内容部署到设备。

继承自 [updatableAssetError](../resources/windowsupdates-updatableasseterror.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|reason|microsoft.graph.windowsUpdates.azureADDeviceRegistrationErrorReason|注册遇到错误的原因。 可取值为：`invalidGlobalDeviceId`、`invalidAzureADDeviceId`、`missingTrustType`、`invalidAzureADJoin`。|

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


---
title: outOfBoxExperienceSettings 资源类型
description: 即开体验设置
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5d2b48fef00c9c3a291a0a2fdfe680b9f4e21030
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404601"
---
# <a name="outofboxexperiencesettings-resource-type"></a>outOfBoxExperienceSettings 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

即开体验设置

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|hidePrivacySettings|Boolean|显示或隐藏给用户的隐私设置|
|hideEULA|Boolean|显示或隐藏 EULA 给用户|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|用户的类型。 可取值为：`administrator`、`standard`。|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|AAD 联接身份验证类型。 可取值为：`singleUser`、`shared`。|
|skipKeyboardSelectionPage|Boolean|如果设置，然后跳过键盘选择页面如果语言和区域设置|
|hideEscapeLink|Boolean|如果设置为 true，然后用户无法通过开始与不同的帐户，请在公司登录|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outOfBoxExperienceSettings",
  "hidePrivacySettings": true,
  "hideEULA": true,
  "userType": "String",
  "deviceUsageType": "String",
  "skipKeyboardSelectionPage": true,
  "hideEscapeLink": true
}
```





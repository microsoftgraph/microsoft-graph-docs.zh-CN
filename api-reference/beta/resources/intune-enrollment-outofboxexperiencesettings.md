---
title: outOfBoxExperienceSettings 资源类型
description: 即开体验设置
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 70f1fb573409a55dd1e586b8e88133c5535de894
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977288"
---
# <a name="outofboxexperiencesettings-resource-type"></a>outOfBoxExperienceSettings 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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

## <a name="relationships"></a>Relationships
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






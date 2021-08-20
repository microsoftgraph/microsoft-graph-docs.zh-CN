---
title: outOfBoxExperienceSettings 资源类型
description: 开箱后体验设置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed86fd6c8d267aa6f12beb5404b9f7a398fb8f4192ad659580dde8c4734443cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239272"
---
# <a name="outofboxexperiencesettings-resource-type"></a>outOfBoxExperienceSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

开箱后体验设置

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|hidePrivacySettings|布尔值|向用户显示或隐藏隐私设置|
|hideEULA|布尔值|向用户显示或隐藏 EULA|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|用户类型。 可取值为：`administrator`、`standard`。|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|AAD 加入身份验证类型。 可取值为：`singleUser`、`shared`。|
|skipKeyboardSelectionPage|布尔值|如果设置，则跳过键盘选择页（如果设置了语言和地区）|
|hideEscapeLink|布尔值|如果设置为 true，则用户无法从公司登录时使用不同的帐户重新开始|

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





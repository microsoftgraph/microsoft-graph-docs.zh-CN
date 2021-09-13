---
title: outOfBoxExperienceSettings 资源类型
description: 开箱后体验设置
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e0caab818558ef9519b2a107b8c8dbecfe6fc71c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039999"
---
# <a name="outofboxexperiencesettings-resource-type"></a>outOfBoxExperienceSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

开箱后体验设置

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|hidePrivacySettings|Boolean|向用户显示或隐藏隐私设置|
|hideEULA|Boolean|向用户显示或隐藏 EULA|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|用户类型。 可取值为：`administrator`、`standard`。|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|AAD 加入身份验证类型。 可取值为：`singleUser`、`shared`。|
|skipKeyboardSelectionPage|Boolean|如果设置，则跳过键盘选择页（如果设置了语言和地区）|
|hideEscapeLink|Boolean|如果设置为 true，则用户无法从公司登录时使用不同的帐户重新开始|

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




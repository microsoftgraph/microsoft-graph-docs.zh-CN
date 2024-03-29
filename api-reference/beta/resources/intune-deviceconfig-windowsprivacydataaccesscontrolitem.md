---
title: windowsPrivacyDataAccessControlItem 资源类型
description: 指定每个隐私数据类别的访问控制级别
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 623e5a363921b1586c131b822d814d8ddf65b9f1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59105906"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a>windowsPrivacyDataAccessControlItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定每个隐私数据类别的访问控制级别

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsPrivacyDataAccessControlItems](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 集合|列出 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象的属性和关系。|
|[获取 windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|读取 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象的属性和关系。|
|[创建 windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|创建新的 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象。|
|[删除 windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|无|删除 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)。|
|[更新 windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|更新 [windowsPrivacyDataAccessControlItem 对象](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|WindowsPrivacyDataAccessControlItem 的键。|
|accessLevel|[windowsPrivacyDataAccessLevel](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|这表示指定应用程序将进入的隐私数据类别的访问级别。 可取值为：`notConfigured`、`forceAllow`、`forceDeny`、`userInControl`。|
|dataCategory|[windowsPrivacyDataCategory](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|这表示将应用特定访问控制的隐私数据类别。 可能的值是 `notConfigured` `accountInfo` `appsRunInBackground` ：、、、、、、、、 `calendar` `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone` `motion` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices` 。|
|appPackageFamilyName|String|应用包系列Windows名称。 设置后，访问级别将应用于指定的应用程序。|
|appDisplayName|String|应用包系列Windows名称。 设置后，访问级别将应用于指定的应用程序。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPrivacyDataAccessControlItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "String (identifier)",
  "accessLevel": "String",
  "dataCategory": "String",
  "appPackageFamilyName": "String",
  "appDisplayName": "String"
}
```




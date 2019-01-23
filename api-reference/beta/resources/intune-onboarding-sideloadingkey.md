---
title: sideLoadingKey 资源类型
description: Windows 8 和租户 8.1 设备安装业务线应用程序需要 SideLoadingKey 实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f7be853faae78e0ac7528d0127fd11b928164ee9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410040"
---
# <a name="sideloadingkey-resource-type"></a>sideLoadingKey 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 8 和租户 8.1 设备安装业务线应用程序需要 SideLoadingKey 实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 sideLoadingKeies](../api/intune-onboarding-sideloadingkey-list.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)集合|列出属性和[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象之间的关系。|
|[获取 sideLoadingKey](../api/intune-onboarding-sideloadingkey-get.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|读取属性和[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的关系。|
|[创建 sideLoadingKey](../api/intune-onboarding-sideloadingkey-create.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|创建新的[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象。|
|[删除 sideLoadingKey](../api/intune-onboarding-sideloadingkey-delete.md)|无|删除[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)。|
|[更新 sideLoadingKey](../api/intune-onboarding-sideloadingkey-update.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|更新[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|端加载关键的唯一 id。|
|值|String|端加载密钥值是 5x5 的值，通过 hiphens 分隔。|
|displayName|String|端加载项显示名称为 it 专业人员管理员。|
|说明|String|显示为 it 专业人员 Admins 端加载项说明正在|
|totalActivation|Int32|端加载项总激活向 it 专业人员 Admins 显示。|
|lastUpdatedDateTime|String|端加载项上次更新日期向 it 专业人员 Admins 显示。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sideLoadingKey"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "String (identifier)",
  "value": "String",
  "displayName": "String",
  "description": "String",
  "totalActivation": 1024,
  "lastUpdatedDateTime": "String"
}
```





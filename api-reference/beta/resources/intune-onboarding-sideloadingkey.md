---
title: sideLoadingKey 资源类型
description: 对于租户, Windows 8 和8.1 设备需要 SideLoadingKey 实体为 intall 的业务线应用程序。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7897a50861910b67763b7d694a30096509c6c56c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170523"
---
# <a name="sideloadingkey-resource-type"></a>sideLoadingKey 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对于租户, Windows 8 和8.1 设备需要 SideLoadingKey 实体为 intall 的业务线应用程序。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 sideLoadingKeies](../api/intune-onboarding-sideloadingkey-list.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)集合|列出[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性和关系。|
|[获取 sideLoadingKey](../api/intune-onboarding-sideloadingkey-get.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|读取[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性和关系。|
|[创建 sideLoadingKey](../api/intune-onboarding-sideloadingkey-create.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|创建新的[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象。|
|[删除 sideLoadingKey](../api/intune-onboarding-sideloadingkey-delete.md)|无|删除[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)。|
|[更新 sideLoadingKey](../api/intune-onboarding-sideloadingkey-update.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|更新[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字串符号|侧加载密钥唯一 Id。|
|值|String|侧加载密钥值, 它是一个5x5 值, 由 hiphens 分隔。|
|displayName|字符串|向 it 专业管理员显示的侧加载密钥名称。|
|说明|字符串|向 it 专业管理员显示的侧加载密钥说明。|
|totalActivation|Int32|向 it 专业管理员显示的端加载密钥总激活数。|
|lastUpdatedDateTime|字符串|向 it 专业管理员显示的侧加载密钥上次更新日期。|

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





---
title: companyPortalBlockedAction 资源类型
description: 按平台和设备所有权类型对公司门户的阻止的操作
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8e456ba03de299a04a1434c7a19871aa908274b1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723769"
---
# <a name="companyportalblockedaction-resource-type"></a>companyPortalBlockedAction 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

按平台和设备所有权类型对公司门户的阻止的操作

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|平台|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|设备 OS/平台。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。|
|所有者|[所有者](../resources/intune-shared-ownertype.md)|设备所有权类型。 可取值为：`unknown`、`company`、`personal`。|
|action|[companyPortalAction](../resources/intune-shared-companyportalaction.md)|设备操作。 可取值为：`unknown`、`remove`、`reset`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.companyPortalBlockedAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.companyPortalBlockedAction",
  "platform": "String",
  "ownerType": "String",
  "action": "String"
}
```






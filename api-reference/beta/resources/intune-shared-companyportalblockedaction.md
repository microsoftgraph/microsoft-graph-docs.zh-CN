---
title: companyPortalBlockedAction 资源类型
description: 按平台和设备所有权类型在公司门户上阻止的操作
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 099f0d5feaa5710cf4d78c3af006d0218c523fa1
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805694"
---
# <a name="companyportalblockedaction-resource-type"></a>companyPortalBlockedAction 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

按平台和设备所有权类型在公司门户上阻止的操作

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|平台|[devicePlatformType](../resources/intune-wip-deviceplatformtype.md)|设备操作系统/平台。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|设备所有权类型。 可取值为：`unknown`、`company`、`personal`。|
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




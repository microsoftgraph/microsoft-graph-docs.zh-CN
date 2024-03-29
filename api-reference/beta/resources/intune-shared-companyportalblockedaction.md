---
title: companyPortalBlockedAction 资源类型
description: 按平台和设备所有权类型在公司门户上阻止的操作
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a8b04ce4697d2ff24f28644908cf12764f8bd3d6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039194"
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




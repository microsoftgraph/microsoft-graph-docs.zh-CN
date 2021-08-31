---
title: securityBaselineContributingPolicy 资源类型
description: 设备设置的安全基线合规性状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 92f49ce93e49524c3a9925e561cae57ca1c49f3d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803789"
---
# <a name="securitybaselinecontributingpolicy-resource-type"></a>securityBaselineContributingPolicy 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备设置的安全基线合规性状态

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|sourceId|String|策略的唯一标识符|
|displayName|String|策略的名称|
|sourceType|[securityBaselinePolicySourceType](../resources/intune-deviceintent-securitybaselinepolicysourcetype.md)|策略的创作源。 可取值为：`deviceConfiguration`、`deviceIntent`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.securityBaselineContributingPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineContributingPolicy",
  "sourceId": "String",
  "displayName": "String",
  "sourceType": "String"
}
```




---
title: zebraFotaArtifact 资源类型
description: 描述特定设备模型的单个项目。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cea341ecb1d3151e8e4f895f6038b7f47cb95cba
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213174"
---
# <a name="zebrafotaartifact-resource-type"></a>zebraFotaArtifact 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述特定设备模型的单个项目。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 zebraFotaArtifacts](../api/intune-androidfotaservice-zebrafotaartifact-list.md)|[zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) 集合|列出 [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) 对象的属性和关系。|
|[获取 zebraFotaArtifact](../api/intune-androidfotaservice-zebrafotaartifact-get.md)|[zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md)|读取 [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) 对象的属性和关系。|
|[创建 zebraFotaArtifact](../api/intune-androidfotaservice-zebrafotaartifact-create.md)|[zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md)|创建新的 [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) 对象。|
|[删除 zebraFotaArtifact](../api/intune-androidfotaservice-zebrafotaartifact-delete.md)|无|删除 [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md)。|
|[更新 zebraFotaArtifact](../api/intune-androidfotaservice-zebrafotaartifact-update.md)|[zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md)|更新 [zebraFotaArtifact 对象的](../resources/intune-androidfotaservice-zebrafotaartifact.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|ZebraFotaArtifact 的 ID。|
|deviceModel|String|项目设备模型。|
|osVersion|String|项目 OS 版本。|
|patchVersion|String|项目修补程序版本。|
|boardSupportPackageVersion|String|开发板支持包的版本。|
|releaseNotesUrl|String|项目发行说明 URL。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.zebraFotaArtifact"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaArtifact",
  "id": "String (identifier)",
  "deviceModel": "String",
  "osVersion": "String",
  "patchVersion": "String",
  "boardSupportPackageVersion": "String",
  "releaseNotesUrl": "String"
}
```





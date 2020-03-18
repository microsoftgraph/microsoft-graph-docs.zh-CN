---
title: teleconferenceDeviceQuality 资源类型
description: 表示视频电话会议设备会话级别质量数据。
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4d76114a35a9ac7d0c9901437b672697c295ebbf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42763268"
---
# <a name="teleconferencedevicequality-resource-type"></a>teleconferenceDeviceQuality 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示视频电话会议设备会话级别质量数据。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|callChainId|Guid|会议中所有参与者调用的唯一标识符，或在 P2P 呼叫中两个参与者呼叫的唯一标识符。 这需要通过复制`Microsoft.Graph.Call.CallChainId`。|
|cloudServiceDeploymentEnvironment|String|部署服务的地理区域，例如`ProdNoam`。|
|cloudServiceDeploymentId|String|由 Azure 分配的唯一部署标识符。|
|cloudServiceInstanceName|String|Azure 部署的云服务实例名称，例如`FrontEnd_IN_3`。|
|cloudServiceName|String|Azure 部署的云服务名称，例如`contoso.cloudapp.net`。|
|deviceDescription|String|任何其他说明，如`VTC Bldg 30/21`。|
|deviceName|String|用户媒体代理名称，例如`Cisco SX80`。|
|mediaLegId|Guid|会议中参与者的特定媒体腿的唯一标识符。  如果发生 retargeting，一个参与者可以有多个媒体支线标识符。 CVI 合作伙伴将分配此值。|
|mediaQualityList|[teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md)集合|媒体会话（呼叫）中的媒体质量列表，例如音频质量、视频质量和/或屏幕共享质量。|
|participantId|Guid|会议中的特定参与者的唯一标识符。 CVI 合作伙伴需要复制`Call.MyParticipantId`到此属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceQuality",
  "baseType": null
}-->

```json
{
  "callChainId": "Guid",
  "cloudServiceDeploymentEnvironment": "String",
  "cloudServiceDeploymentId": "String",
  "cloudServiceInstanceName": "String",
  "cloudServiceName": "String",
  "deviceDescription": "String",
  "deviceName": "String",
  "mediaLegId": "Guid",
  "mediaQualityList": [{"@odata.type": "microsoft.graph.teleconferenceDeviceMediaQuality"}],
  "participantId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teleconferenceDeviceQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: remoteAssistancePartner 资源类型
description: remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b0bdbffc33358770b43ac67dcb67d9acea7655f0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407933"
---
# <a name="remoteassistancepartner-resource-type"></a>remoteAssistancePartner 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 remoteAssistancePartners](../api/intune-remoteassistance-remoteassistancepartner-list.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合|列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。|
|[获取 remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。|
|[创建 remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。|
|[删除 remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|无|删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。|
|[更新 remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。|
|[beginOnboarding 操作](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|无|尚未记录|
|[断开连接操作](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|合作伙伴的唯一标识符。|
|displayName|String|合作伙伴的显示名称。|
|onboardingUrl|String|合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|TBD。 可取值为：`notOnboarded`、`onboarding`、`onboarded`。|
|lastConnectionDateTime|DateTimeOffset|TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```





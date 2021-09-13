---
title: remoteAssistancePartner 资源类型
description: RemoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cff6814d954003a5a77a7c9df5c9961d1bcebe7a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039495"
---
# <a name="remoteassistancepartner-resource-type"></a>remoteAssistancePartner 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

RemoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 remoteAssistancePartners](../api/intune-remoteassistance-remoteassistancepartner-list.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合|列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。|
|[获取 remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。|
|[创建 remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。|
|[删除 remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|无|删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。|
|[更新 remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。|
|[beginOnboarding 操作](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|无|开始载入的请求。  必须与相应的 TeamViewer 帐户信息结合|
|[断开连接操作](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|无|删除活动 TeamViewer 连接器的请求|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|合作伙伴的唯一标识符。|
|displayName|String|合作伙伴的显示名称。|
|onboardingUrl|String|合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|当前 TeamViewer 连接器状态的友好说明。 可取值为：`notOnboarded`、`onboarding`、`onboarded`。|
|lastConnectionDateTime|DateTimeOffset|TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。|
|onboardingRequestExpiryDateTime|DateTimeOffset|当 OnboardingStatus 载入时，这是载入请求到期的日期时间。|

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
  "lastConnectionDateTime": "String (timestamp)",
  "onboardingRequestExpiryDateTime": "String (timestamp)"
}
```




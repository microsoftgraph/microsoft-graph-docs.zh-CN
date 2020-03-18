---
title: remoteAssistancePartner 资源类型
description: RemoteAssistPartner 资源表示给定的远程协助合作伙伴服务的元数据和状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b85cd11112045df5ff2babfee5f8b51dec57c0d6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772809"
---
# <a name="remoteassistancepartner-resource-type"></a>remoteAssistancePartner 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

RemoteAssistPartner 资源表示给定的远程协助合作伙伴服务的元数据和状态。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 remoteAssistancePartners](../api/intune-remoteassistance-remoteassistancepartner-list.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合|列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。|
|[获取 remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。|
|[创建 remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。|
|[删除 remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|无|删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。|
|[更新 remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。|
|[beginOnboarding 操作](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|None|启动 "加入" 的请求。  必须与相应的 TeamViewer 帐户信息结合使用|
|[断开连接操作](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|无|请求删除活动的 TeamViewer 连接器|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|合作伙伴的唯一标识符。|
|displayName|字符串|合作伙伴的显示名称。|
|onboardingUrl|String|合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|当前 TeamViewer 连接器状态的友好说明。 可取值为：`notOnboarded`、`onboarding`、`onboarded`。|
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




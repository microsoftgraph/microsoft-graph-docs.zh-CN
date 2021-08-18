---
title: adminConsent 资源类型
description: 管理员同意信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d56646299766427a4598ab1073064bfa8ea86a3c405df17b59bb52866b47e75a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227363"
---
# <a name="adminconsent-resource-type"></a>adminConsent 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理员同意信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|shareAPNSData|[adminConsentState](../resources/intune-devices-adminconsentstate.md)|管理员同意将用户和设备数据共享到 Apple 的状态。 可取值为：`notConfigured`、`granted`、`notGranted`。|
|shareUserExperienceAnalyticsData|[adminConsentState](../resources/intune-devices-adminconsentstate.md)|获取或设置共享用户体验分析数据的管理员同意。 可取值为：`notConfigured`、`granted`、`notGranted`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String",
  "shareUserExperienceAnalyticsData": "String"
}
```





---
title: teamworkOnPremisesCalendarSyncConfiguration 资源类型
description: 表示用于同步启用了日历的设备Microsoft Teams客户端Microsoft Teams的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7b5b8d95cc2743b15c6903852a0d81c41949148a
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262333"
---
# <a name="teamworkonpremisescalendarsyncconfiguration-resource-type"></a>teamworkOnPremisesCalendarSyncConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用于同步启用了日历的设备Microsoft Teams客户端[Microsoft Teams的详细信息。](../resources/teamworkdevice.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|domain|String|完全限定的域名 (FQDN) 的Skype for Business Server。 如果Exchange SIP 域Skype for Business SIP 域与用户Exchange域不同，请使用该 SIP 域。|
|domainUserName|String|控制台设备的域和用户名，例如， `Seattle\RanierConf`。|
|smtpAddress|String|简单邮件传输协议 (SMTP) 用户帐户的地址。 只有在使用 UPN 帐户和 UPN (不同的用户主体) ，才需要Exchange用户主体Microsoft Teams和Skype for Business。 在混合环境中，这是一种常见方案，其中Exchange服务器。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkOnPremisesCalendarSyncConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkOnPremisesCalendarSyncConfiguration",
  "domain": "String",
  "domainUserName": "String",
  "smtpAddress": "String"
}
```


---
title: aadUserNotificationRecipient 资源类型
description: 表示 Azure AD Azure Active Directory (订阅) 订阅源中发送的通知的用户Microsoft Teams收件人。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ec8e05a09af27ca6092da24e13a604fdd7e013f4
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813193"
---
# <a name="aadusernotificationrecipient-resource-type"></a>aadUserNotificationRecipient 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure AD Azure Active Directory (订阅) 订阅源中发送的通知的用户Microsoft Teams收件人。

继承自 [teamworkNotificationRecipient](teamworknotificationrecipient.md)。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|userId|String|Azure AD 用户标识符。 使用 [List users](../api/user-list.md) 方法可获取此 ID。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.aadUserNotificationRecipient"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aadUserNotificationRecipient",
  "userId": "String"
}
```


---
title: aadUserNotificationRecipient 资源类型
description: 表示在 Microsoft 团队活动源中发送的通知的 Azure Active Directory (Azure AD) 用户收件人。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 118951336a031548a557f94df8b2b2068e415408
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377515"
---
# <a name="aadusernotificationrecipient-resource-type"></a>aadUserNotificationRecipient 资源类型

命名空间：microsoft.graph

表示在 Microsoft 团队活动源中发送的通知的 Azure Active Directory (Azure AD) 用户收件人。

继承自 [teamworkNotificationRecipient](teamworknotificationrecipient.md)。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|userId|字符串|Azure AD 用户标识符。 使用 [List users](../api/user-list.md) 方法获取此 ID。|

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


---
title: aadUserNotificationRecipient 资源类型
description: 表示 Azure AD Azure Active Directory (订阅) 订阅源中发送的通知的用户Microsoft Teams收件人。
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: bb5d95c36fb362af6d4f66c1e18a4dcb768c1b204a4e2f70f24f5afe80545483
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230849"
---
# <a name="aadusernotificationrecipient-resource-type"></a>aadUserNotificationRecipient 资源类型

命名空间：microsoft.graph

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


---
title: aadUserNotificationRecipient 资源类型
description: 表示 Azure AD Azure Active Directory (订阅) 订阅源中发送的通知的用户Microsoft Teams收件人。
author: eddie-lee-msft
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4588b0d17dc099ee65cedeba52bd5cbd1edf7bae
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021783"
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


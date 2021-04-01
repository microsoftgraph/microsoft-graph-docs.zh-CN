---
title: aadUserNotificationRecipient 资源类型
description: 表示 Azure AD (Azure Active Directory) Microsoft Teams 活动源中发送的通知的用户收件人。
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dadb08dad99f6c4fd6857e8e60f457ea51811de1
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51474123"
---
# <a name="aadusernotificationrecipient-resource-type"></a>aadUserNotificationRecipient 资源类型

命名空间：microsoft.graph

表示 Azure AD (Azure Active Directory) Microsoft Teams 活动源中发送的通知的用户收件人。

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


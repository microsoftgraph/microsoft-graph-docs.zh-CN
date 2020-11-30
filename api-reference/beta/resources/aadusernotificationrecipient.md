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
# <a name="aadusernotificationrecipient-resource-type"></a><span data-ttu-id="193db-103">aadUserNotificationRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="193db-103">aadUserNotificationRecipient resource type</span></span>

<span data-ttu-id="193db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="193db-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="193db-105">表示在 Microsoft 团队活动源中发送的通知的 Azure Active Directory (Azure AD) 用户收件人。</span><span class="sxs-lookup"><span data-stu-id="193db-105">Represents an Azure Active Directory (Azure AD) user recipient of a notification sent in a Microsoft Teams activity feed.</span></span>

<span data-ttu-id="193db-106">继承自 [teamworkNotificationRecipient](teamworknotificationrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="193db-106">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="193db-107">属性</span><span class="sxs-lookup"><span data-stu-id="193db-107">Properties</span></span>
|<span data-ttu-id="193db-108">属性</span><span class="sxs-lookup"><span data-stu-id="193db-108">Property</span></span>|<span data-ttu-id="193db-109">类型</span><span class="sxs-lookup"><span data-stu-id="193db-109">Type</span></span>|<span data-ttu-id="193db-110">描述</span><span class="sxs-lookup"><span data-stu-id="193db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="193db-111">userId</span><span class="sxs-lookup"><span data-stu-id="193db-111">userId</span></span>|<span data-ttu-id="193db-112">字符串</span><span class="sxs-lookup"><span data-stu-id="193db-112">String</span></span>|<span data-ttu-id="193db-113">Azure AD 用户标识符。</span><span class="sxs-lookup"><span data-stu-id="193db-113">Azure AD user identifier.</span></span> <span data-ttu-id="193db-114">使用 [List users](../api/user-list.md) 方法获取此 ID。</span><span class="sxs-lookup"><span data-stu-id="193db-114">Use the [List users](../api/user-list.md) method to get this ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="193db-115">关系</span><span class="sxs-lookup"><span data-stu-id="193db-115">Relationships</span></span>
<span data-ttu-id="193db-116">无。</span><span class="sxs-lookup"><span data-stu-id="193db-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="193db-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="193db-117">JSON representation</span></span>
<span data-ttu-id="193db-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="193db-118">The following is a JSON representation of the resource.</span></span>
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


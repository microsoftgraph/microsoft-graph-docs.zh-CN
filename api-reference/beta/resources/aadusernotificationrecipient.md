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
# <a name="aadusernotificationrecipient-resource-type"></a><span data-ttu-id="24dd0-103">aadUserNotificationRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="24dd0-103">aadUserNotificationRecipient resource type</span></span>

<span data-ttu-id="24dd0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24dd0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24dd0-105">表示 Azure AD Azure Active Directory (订阅) 订阅源中发送的通知的用户Microsoft Teams收件人。</span><span class="sxs-lookup"><span data-stu-id="24dd0-105">Represents an Azure Active Directory (Azure AD) user recipient of a notification sent in a Microsoft Teams activity feed.</span></span>

<span data-ttu-id="24dd0-106">继承自 [teamworkNotificationRecipient](teamworknotificationrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="24dd0-106">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="24dd0-107">属性</span><span class="sxs-lookup"><span data-stu-id="24dd0-107">Properties</span></span>
|<span data-ttu-id="24dd0-108">属性</span><span class="sxs-lookup"><span data-stu-id="24dd0-108">Property</span></span>|<span data-ttu-id="24dd0-109">类型</span><span class="sxs-lookup"><span data-stu-id="24dd0-109">Type</span></span>|<span data-ttu-id="24dd0-110">描述</span><span class="sxs-lookup"><span data-stu-id="24dd0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24dd0-111">userId</span><span class="sxs-lookup"><span data-stu-id="24dd0-111">userId</span></span>|<span data-ttu-id="24dd0-112">String</span><span class="sxs-lookup"><span data-stu-id="24dd0-112">String</span></span>|<span data-ttu-id="24dd0-113">Azure AD 用户标识符。</span><span class="sxs-lookup"><span data-stu-id="24dd0-113">Azure AD user identifier.</span></span> <span data-ttu-id="24dd0-114">使用 [List users](../api/user-list.md) 方法可获取此 ID。</span><span class="sxs-lookup"><span data-stu-id="24dd0-114">Use the [List users](../api/user-list.md) method to get this ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24dd0-115">关系</span><span class="sxs-lookup"><span data-stu-id="24dd0-115">Relationships</span></span>
<span data-ttu-id="24dd0-116">无。</span><span class="sxs-lookup"><span data-stu-id="24dd0-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="24dd0-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24dd0-117">JSON representation</span></span>
<span data-ttu-id="24dd0-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24dd0-118">The following is a JSON representation of the resource.</span></span>
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


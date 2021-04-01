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
# <a name="aadusernotificationrecipient-resource-type"></a><span data-ttu-id="aaab5-103">aadUserNotificationRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="aaab5-103">aadUserNotificationRecipient resource type</span></span>

<span data-ttu-id="aaab5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaab5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aaab5-105">表示 Azure AD (Azure Active Directory) Microsoft Teams 活动源中发送的通知的用户收件人。</span><span class="sxs-lookup"><span data-stu-id="aaab5-105">Represents an Azure Active Directory (Azure AD) user recipient of a notification sent in a Microsoft Teams activity feed.</span></span>

<span data-ttu-id="aaab5-106">继承自 [teamworkNotificationRecipient](teamworknotificationrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="aaab5-106">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="aaab5-107">属性</span><span class="sxs-lookup"><span data-stu-id="aaab5-107">Properties</span></span>
|<span data-ttu-id="aaab5-108">属性</span><span class="sxs-lookup"><span data-stu-id="aaab5-108">Property</span></span>|<span data-ttu-id="aaab5-109">类型</span><span class="sxs-lookup"><span data-stu-id="aaab5-109">Type</span></span>|<span data-ttu-id="aaab5-110">描述</span><span class="sxs-lookup"><span data-stu-id="aaab5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaab5-111">userId</span><span class="sxs-lookup"><span data-stu-id="aaab5-111">userId</span></span>|<span data-ttu-id="aaab5-112">String</span><span class="sxs-lookup"><span data-stu-id="aaab5-112">String</span></span>|<span data-ttu-id="aaab5-113">Azure AD 用户标识符。</span><span class="sxs-lookup"><span data-stu-id="aaab5-113">Azure AD user identifier.</span></span> <span data-ttu-id="aaab5-114">使用 [List users](../api/user-list.md) 方法可获取此 ID。</span><span class="sxs-lookup"><span data-stu-id="aaab5-114">Use the [List users](../api/user-list.md) method to get this ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aaab5-115">关系</span><span class="sxs-lookup"><span data-stu-id="aaab5-115">Relationships</span></span>
<span data-ttu-id="aaab5-116">无。</span><span class="sxs-lookup"><span data-stu-id="aaab5-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aaab5-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aaab5-117">JSON representation</span></span>
<span data-ttu-id="aaab5-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aaab5-118">The following is a JSON representation of the resource.</span></span>
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


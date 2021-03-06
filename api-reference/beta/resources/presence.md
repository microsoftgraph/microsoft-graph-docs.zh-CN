---
title: 状态资源类型
description: 包含有关用户状态的信息，包括其可用性和用户活动。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: d6f88f23a6c08d5aa757163d4956c104a603e87b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515623"
---
# <a name="presence-resource-type"></a><span data-ttu-id="e4bba-103">状态资源类型</span><span class="sxs-lookup"><span data-stu-id="e4bba-103">presence resource type</span></span>

<span data-ttu-id="e4bba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4bba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4bba-105">包含有关用户状态的信息，包括其可用性和用户活动。</span><span class="sxs-lookup"><span data-stu-id="e4bba-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="e4bba-106">**注意：** 此资源当前仅受 Microsoft Teams 用户支持。</span><span class="sxs-lookup"><span data-stu-id="e4bba-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="e4bba-107">此资源支持订阅 [更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="e4bba-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="e4bba-108">方法</span><span class="sxs-lookup"><span data-stu-id="e4bba-108">Methods</span></span>

| <span data-ttu-id="e4bba-109">方法</span><span class="sxs-lookup"><span data-stu-id="e4bba-109">Method</span></span>                                                            | <span data-ttu-id="e4bba-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e4bba-110">Return Type</span></span>                                       | <span data-ttu-id="e4bba-111">说明</span><span class="sxs-lookup"><span data-stu-id="e4bba-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="e4bba-112">获取状态</span><span class="sxs-lookup"><span data-stu-id="e4bba-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="e4bba-113">状态</span><span class="sxs-lookup"><span data-stu-id="e4bba-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="e4bba-114">获取用户状态信息。</span><span class="sxs-lookup"><span data-stu-id="e4bba-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="e4bba-115">获取多个用户状态</span><span class="sxs-lookup"><span data-stu-id="e4bba-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="e4bba-116">[presence](../resources/presence.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e4bba-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="e4bba-117">获取多个用户状态信息。</span><span class="sxs-lookup"><span data-stu-id="e4bba-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="e4bba-118">属性</span><span class="sxs-lookup"><span data-stu-id="e4bba-118">Properties</span></span>

| <span data-ttu-id="e4bba-119">关系</span><span class="sxs-lookup"><span data-stu-id="e4bba-119">Relationship</span></span>        | <span data-ttu-id="e4bba-120">类型</span><span class="sxs-lookup"><span data-stu-id="e4bba-120">Type</span></span>                                                 | <span data-ttu-id="e4bba-121">说明</span><span class="sxs-lookup"><span data-stu-id="e4bba-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="e4bba-122">id</span><span class="sxs-lookup"><span data-stu-id="e4bba-122">id</span></span>    |  <span data-ttu-id="e4bba-123">string</span><span class="sxs-lookup"><span data-stu-id="e4bba-123">string</span></span>     |  <span data-ttu-id="e4bba-124">用户对象 ID</span><span class="sxs-lookup"><span data-stu-id="e4bba-124">The user object id</span></span>   |
|<span data-ttu-id="e4bba-125">availability</span><span class="sxs-lookup"><span data-stu-id="e4bba-125">availability</span></span>    |  <span data-ttu-id="e4bba-126">字符串集合</span><span class="sxs-lookup"><span data-stu-id="e4bba-126">string collection</span></span>   |   <span data-ttu-id="e4bba-127">用户的基本状态信息。</span><span class="sxs-lookup"><span data-stu-id="e4bba-127">The base presence information for a user.</span></span> <span data-ttu-id="e4bba-128">可能的值是 `Available` ， ， ， ， ， ， `AvailableIdle` `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` ， `Offline``PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="e4bba-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="e4bba-129">活动</span><span class="sxs-lookup"><span data-stu-id="e4bba-129">activity</span></span>    |  <span data-ttu-id="e4bba-130">字符串集合</span><span class="sxs-lookup"><span data-stu-id="e4bba-130">string collection</span></span>      |    <span data-ttu-id="e4bba-131">用户可用性的补充信息。</span><span class="sxs-lookup"><span data-stu-id="e4bba-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="e4bba-132">可能的值是 `Available` ， ， ， ， ， ， ， `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` 。</span><span class="sxs-lookup"><span data-stu-id="e4bba-132">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |
|<span data-ttu-id="e4bba-133">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="e4bba-133">outOfOfficeSettings</span></span> | [<span data-ttu-id="e4bba-134">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="e4bba-134">outOfOfficeSettings</span></span>](outOfOfficeSettings.md) | <span data-ttu-id="e4bba-135">用户的外出设置。</span><span class="sxs-lookup"><span data-stu-id="e4bba-135">The out of office settings for a user.</span></span> |

><span data-ttu-id="e4bba-136">**注意：** 若要详细了解不同的状态，请参阅 [Teams 中的用户状态](/microsoftteams/presence-admins)。</span><span class="sxs-lookup"><span data-stu-id="e4bba-136">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="e4bba-137">关系</span><span class="sxs-lookup"><span data-stu-id="e4bba-137">Relationships</span></span>

<span data-ttu-id="e4bba-138">无。</span><span class="sxs-lookup"><span data-stu-id="e4bba-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4bba-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4bba-139">JSON representation</span></span>

<span data-ttu-id="e4bba-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4bba-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.presence"
}-->
```json
{
   "id":"string",
   "availability":"string",
   "activity":"string",
   "outOfOfficeSettings":{"@odata.type": "#microsoft.graph.outOfOfficeSettings"}
}
```

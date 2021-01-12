---
title: 状态资源类型
description: 包含有关用户状态的信息，包括其可用性和用户活动。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: ddbe555df37d232940bb8eadb081be459d0f8562
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796575"
---
# <a name="presence-resource-type"></a><span data-ttu-id="dcdb5-103">状态资源类型</span><span class="sxs-lookup"><span data-stu-id="dcdb5-103">presence resource type</span></span>

<span data-ttu-id="dcdb5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcdb5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dcdb5-105">包含有关用户状态的信息，包括其可用性和用户活动。</span><span class="sxs-lookup"><span data-stu-id="dcdb5-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="dcdb5-106">**注意：** 此资源当前仅受 Microsoft Teams 用户支持。</span><span class="sxs-lookup"><span data-stu-id="dcdb5-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="dcdb5-107">此资源支持订阅 [更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="dcdb5-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="dcdb5-108">方法</span><span class="sxs-lookup"><span data-stu-id="dcdb5-108">Methods</span></span>

| <span data-ttu-id="dcdb5-109">方法</span><span class="sxs-lookup"><span data-stu-id="dcdb5-109">Method</span></span>                                                            | <span data-ttu-id="dcdb5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="dcdb5-110">Return Type</span></span>                                       | <span data-ttu-id="dcdb5-111">说明</span><span class="sxs-lookup"><span data-stu-id="dcdb5-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="dcdb5-112">获取状态</span><span class="sxs-lookup"><span data-stu-id="dcdb5-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="dcdb5-113">状态</span><span class="sxs-lookup"><span data-stu-id="dcdb5-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="dcdb5-114">获取用户状态信息。</span><span class="sxs-lookup"><span data-stu-id="dcdb5-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="dcdb5-115">获取多个用户状态</span><span class="sxs-lookup"><span data-stu-id="dcdb5-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="dcdb5-116">[presence](../resources/presence.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dcdb5-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="dcdb5-117">获取多个用户状态信息。</span><span class="sxs-lookup"><span data-stu-id="dcdb5-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="dcdb5-118">属性</span><span class="sxs-lookup"><span data-stu-id="dcdb5-118">Properties</span></span>

| <span data-ttu-id="dcdb5-119">关系</span><span class="sxs-lookup"><span data-stu-id="dcdb5-119">Relationship</span></span>        | <span data-ttu-id="dcdb5-120">类型</span><span class="sxs-lookup"><span data-stu-id="dcdb5-120">Type</span></span>                                                 | <span data-ttu-id="dcdb5-121">说明</span><span class="sxs-lookup"><span data-stu-id="dcdb5-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="dcdb5-122">id</span><span class="sxs-lookup"><span data-stu-id="dcdb5-122">id</span></span>    |  <span data-ttu-id="dcdb5-123">string</span><span class="sxs-lookup"><span data-stu-id="dcdb5-123">string</span></span>     |  <span data-ttu-id="dcdb5-124">用户对象 ID</span><span class="sxs-lookup"><span data-stu-id="dcdb5-124">The user object id</span></span>   |
|<span data-ttu-id="dcdb5-125">availability</span><span class="sxs-lookup"><span data-stu-id="dcdb5-125">availability</span></span>    |  <span data-ttu-id="dcdb5-126">string 集合</span><span class="sxs-lookup"><span data-stu-id="dcdb5-126">string collection</span></span>   |   <span data-ttu-id="dcdb5-127">用户的基本状态信息。</span><span class="sxs-lookup"><span data-stu-id="dcdb5-127">The base presence information for a user.</span></span> <span data-ttu-id="dcdb5-128">可能的值是 `Available` `AvailableIdle` ， `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline``PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="dcdb5-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="dcdb5-129">活动</span><span class="sxs-lookup"><span data-stu-id="dcdb5-129">activity</span></span>    |  <span data-ttu-id="dcdb5-130">string 集合</span><span class="sxs-lookup"><span data-stu-id="dcdb5-130">string collection</span></span>      |    <span data-ttu-id="dcdb5-131">用户可用性的补充信息。</span><span class="sxs-lookup"><span data-stu-id="dcdb5-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="dcdb5-132">可能的值是 ， 。 `Available` `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly`</span><span class="sxs-lookup"><span data-stu-id="dcdb5-132">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |
|<span data-ttu-id="dcdb5-133">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="dcdb5-133">outOfOfficeSettings</span></span> | [<span data-ttu-id="dcdb5-134">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="dcdb5-134">outOfOfficeSettings</span></span>](outOfOfficeSettings.md) | <span data-ttu-id="dcdb5-135">用户的外出设置。</span><span class="sxs-lookup"><span data-stu-id="dcdb5-135">The out of office settings for a user.</span></span> |

><span data-ttu-id="dcdb5-136">**注意：** 若要详细了解不同的状态，请参阅 [Teams 中的用户状态](/microsoftteams/presence-admins)。</span><span class="sxs-lookup"><span data-stu-id="dcdb5-136">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="dcdb5-137">关系</span><span class="sxs-lookup"><span data-stu-id="dcdb5-137">Relationships</span></span>

<span data-ttu-id="dcdb5-138">无。</span><span class="sxs-lookup"><span data-stu-id="dcdb5-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcdb5-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dcdb5-139">JSON representation</span></span>

<span data-ttu-id="dcdb5-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dcdb5-140">The following is a JSON representation of the resource.</span></span>

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

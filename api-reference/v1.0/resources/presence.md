---
title: 状态资源类型
description: 包含有关用户状态的信息，包括用户的可用性和用户活动。
author: elvinyang-msft
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 52c726ab1e5b9d50a81797bc2d2375bee3793a2a
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581204"
---
# <a name="presence-resource-type"></a><span data-ttu-id="1c487-103">状态资源类型</span><span class="sxs-lookup"><span data-stu-id="1c487-103">presence resource type</span></span>

<span data-ttu-id="1c487-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c487-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c487-105">包含有关用户状态的信息，包括用户的可用性和用户活动。</span><span class="sxs-lookup"><span data-stu-id="1c487-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="1c487-106">**注意：** 此资源目前仅对 Microsoft 团队用户受支持。</span><span class="sxs-lookup"><span data-stu-id="1c487-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="1c487-107">此资源支持订阅 [更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="1c487-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="1c487-108">方法</span><span class="sxs-lookup"><span data-stu-id="1c487-108">Methods</span></span>

| <span data-ttu-id="1c487-109">方法</span><span class="sxs-lookup"><span data-stu-id="1c487-109">Method</span></span>                                                            | <span data-ttu-id="1c487-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1c487-110">Return Type</span></span>                                       | <span data-ttu-id="1c487-111">Description</span><span class="sxs-lookup"><span data-stu-id="1c487-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="1c487-112">获取状态</span><span class="sxs-lookup"><span data-stu-id="1c487-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="1c487-113">状态</span><span class="sxs-lookup"><span data-stu-id="1c487-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="1c487-114">获取用户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="1c487-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="1c487-115">获取多个用户的状态</span><span class="sxs-lookup"><span data-stu-id="1c487-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="1c487-116">[状态](../resources/presence.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c487-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="1c487-117">获取多个用户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="1c487-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="1c487-118">属性</span><span class="sxs-lookup"><span data-stu-id="1c487-118">Properties</span></span>

| <span data-ttu-id="1c487-119">关系</span><span class="sxs-lookup"><span data-stu-id="1c487-119">Relationship</span></span>        | <span data-ttu-id="1c487-120">类型</span><span class="sxs-lookup"><span data-stu-id="1c487-120">Type</span></span>                                                 | <span data-ttu-id="1c487-121">说明</span><span class="sxs-lookup"><span data-stu-id="1c487-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="1c487-122">id</span><span class="sxs-lookup"><span data-stu-id="1c487-122">id</span></span>    |  <span data-ttu-id="1c487-123">string</span><span class="sxs-lookup"><span data-stu-id="1c487-123">string</span></span>     |  <span data-ttu-id="1c487-124">User 对象 id</span><span class="sxs-lookup"><span data-stu-id="1c487-124">The user object id</span></span>   |
|<span data-ttu-id="1c487-125">availability</span><span class="sxs-lookup"><span data-stu-id="1c487-125">availability</span></span>    |  <span data-ttu-id="1c487-126">字符串集合</span><span class="sxs-lookup"><span data-stu-id="1c487-126">string collection</span></span>   |   <span data-ttu-id="1c487-127">用户的基本状态信息。</span><span class="sxs-lookup"><span data-stu-id="1c487-127">The base presence information for a user.</span></span> <span data-ttu-id="1c487-128">可能的值为、、、、、、、 `Available` `AvailableIdle` `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline``PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="1c487-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="1c487-129">activity</span><span class="sxs-lookup"><span data-stu-id="1c487-129">activity</span></span>    |  <span data-ttu-id="1c487-130">字符串集合</span><span class="sxs-lookup"><span data-stu-id="1c487-130">string collection</span></span>      |    <span data-ttu-id="1c487-131">将补充信息提供给用户的可用性。</span><span class="sxs-lookup"><span data-stu-id="1c487-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="1c487-132">可能的值为、、、、、、、、、、、、、、 `Available` `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` 。</span><span class="sxs-lookup"><span data-stu-id="1c487-132">Possible values are `Available`, `Away`, `BeRightBack`,`Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="1c487-133">**注意：** 若要了解有关不同状态的详细信息，请参阅 [团队中的用户状态](/microsoftteams/presence-admins)。</span><span class="sxs-lookup"><span data-stu-id="1c487-133">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="1c487-134">关系</span><span class="sxs-lookup"><span data-stu-id="1c487-134">Relationships</span></span>

<span data-ttu-id="1c487-135">无。</span><span class="sxs-lookup"><span data-stu-id="1c487-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c487-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c487-136">JSON representation</span></span>

<span data-ttu-id="1c487-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c487-137">The following is a JSON representation of the resource.</span></span>

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
   "activity":"string"
}
```
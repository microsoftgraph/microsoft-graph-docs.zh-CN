---
title: 状态资源类型
description: 包含有关用户状态的信息，包括用户的可用性和用户活动。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 797ddac8bc582cd5e5d4d51e0e1ad94645c3c1e0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521570"
---
# <a name="presence-resource-type"></a><span data-ttu-id="59f6e-103">状态资源类型</span><span class="sxs-lookup"><span data-stu-id="59f6e-103">presence resource type</span></span>

<span data-ttu-id="59f6e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="59f6e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="59f6e-105">包含有关用户状态的信息，包括用户的可用性和用户活动。</span><span class="sxs-lookup"><span data-stu-id="59f6e-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="59f6e-106">**注意：** 此资源目前仅对 Microsoft 团队用户受支持。</span><span class="sxs-lookup"><span data-stu-id="59f6e-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

## <a name="methods"></a><span data-ttu-id="59f6e-107">方法</span><span class="sxs-lookup"><span data-stu-id="59f6e-107">Methods</span></span>

| <span data-ttu-id="59f6e-108">方法</span><span class="sxs-lookup"><span data-stu-id="59f6e-108">Method</span></span>                                                            | <span data-ttu-id="59f6e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="59f6e-109">Return Type</span></span>                                       | <span data-ttu-id="59f6e-110">说明</span><span class="sxs-lookup"><span data-stu-id="59f6e-110">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="59f6e-111">获取状态</span><span class="sxs-lookup"><span data-stu-id="59f6e-111">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="59f6e-112">状态</span><span class="sxs-lookup"><span data-stu-id="59f6e-112">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="59f6e-113">获取用户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="59f6e-113">Get a user's presence information.</span></span>
| [<span data-ttu-id="59f6e-114">获取多个用户的状态</span><span class="sxs-lookup"><span data-stu-id="59f6e-114">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="59f6e-115">[状态](../resources/presence.md)集合</span><span class="sxs-lookup"><span data-stu-id="59f6e-115">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="59f6e-116">获取多个用户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="59f6e-116">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="59f6e-117">属性</span><span class="sxs-lookup"><span data-stu-id="59f6e-117">Properties</span></span>

| <span data-ttu-id="59f6e-118">关系</span><span class="sxs-lookup"><span data-stu-id="59f6e-118">Relationship</span></span>        | <span data-ttu-id="59f6e-119">类型</span><span class="sxs-lookup"><span data-stu-id="59f6e-119">Type</span></span>                                                 | <span data-ttu-id="59f6e-120">说明</span><span class="sxs-lookup"><span data-stu-id="59f6e-120">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="59f6e-121">id</span><span class="sxs-lookup"><span data-stu-id="59f6e-121">id</span></span>    |  <span data-ttu-id="59f6e-122">string</span><span class="sxs-lookup"><span data-stu-id="59f6e-122">string</span></span>     |  <span data-ttu-id="59f6e-123">User 对象 id</span><span class="sxs-lookup"><span data-stu-id="59f6e-123">The user object id</span></span>   |
|<span data-ttu-id="59f6e-124">availability</span><span class="sxs-lookup"><span data-stu-id="59f6e-124">availability</span></span>    |  <span data-ttu-id="59f6e-125">string 集合</span><span class="sxs-lookup"><span data-stu-id="59f6e-125">string collection</span></span>   |   <span data-ttu-id="59f6e-126">用户的基本状态信息。</span><span class="sxs-lookup"><span data-stu-id="59f6e-126">The base presence information for a user.</span></span> <span data-ttu-id="59f6e-127">可能的值`Available`为`AvailableIdle`、 `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb`、、、、 `Offline`、、`PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="59f6e-127">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="59f6e-128">activity</span><span class="sxs-lookup"><span data-stu-id="59f6e-128">activity</span></span>    |  <span data-ttu-id="59f6e-129">string 集合</span><span class="sxs-lookup"><span data-stu-id="59f6e-129">string collection</span></span>      |    <span data-ttu-id="59f6e-130">将补充信息提供给用户的可用性。</span><span class="sxs-lookup"><span data-stu-id="59f6e-130">The supplemental information to a user's availability.</span></span> <span data-ttu-id="59f6e-131">可能的值`Available`为`Away`、 `BeRightBack``Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `UrgentInterruptionsOnly`、、`InAMeeting`、、、、、、、、、、、。 `Offline` `OffWork``OutOfOffice` `PresenceUnknown``Presenting`</span><span class="sxs-lookup"><span data-stu-id="59f6e-131">Possible values are `Available`, `Away`, `BeRightBack`,`Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="59f6e-132">**注意：** 若要了解有关不同状态的详细信息，请参阅[团队中的用户状态](https://docs.microsoft.com/microsoftteams/presence-admins)。</span><span class="sxs-lookup"><span data-stu-id="59f6e-132">**Note:** To learn more about the different presence states, see [User presence in Teams](https://docs.microsoft.com/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="59f6e-133">关系</span><span class="sxs-lookup"><span data-stu-id="59f6e-133">Relationships</span></span>

<span data-ttu-id="59f6e-134">无。</span><span class="sxs-lookup"><span data-stu-id="59f6e-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59f6e-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59f6e-135">JSON representation</span></span>

<span data-ttu-id="59f6e-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59f6e-136">The following is a JSON representation of the resource.</span></span>

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

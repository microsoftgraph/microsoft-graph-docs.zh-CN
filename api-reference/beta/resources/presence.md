---
title: 状态资源类型
description: 包含有关用户状态的信息，包括用户的可用性和用户活动。
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 15635f29143a51f87a107c5f4e632b8684e79c50
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844279"
---
# <a name="presence-resource-type"></a><span data-ttu-id="3f212-103">状态资源类型</span><span class="sxs-lookup"><span data-stu-id="3f212-103">presence resource type</span></span>

<span data-ttu-id="3f212-104">包含有关用户状态的信息，包括用户的可用性和用户活动。</span><span class="sxs-lookup"><span data-stu-id="3f212-104">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="3f212-105">**注意：** 此资源目前仅对 Microsoft 团队用户受支持。</span><span class="sxs-lookup"><span data-stu-id="3f212-105">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

## <a name="methods"></a><span data-ttu-id="3f212-106">方法</span><span class="sxs-lookup"><span data-stu-id="3f212-106">Methods</span></span>

| <span data-ttu-id="3f212-107">方法</span><span class="sxs-lookup"><span data-stu-id="3f212-107">Method</span></span>                                                            | <span data-ttu-id="3f212-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f212-108">Return Type</span></span>                                       | <span data-ttu-id="3f212-109">说明</span><span class="sxs-lookup"><span data-stu-id="3f212-109">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="3f212-110">获取状态</span><span class="sxs-lookup"><span data-stu-id="3f212-110">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="3f212-111">shell</span><span class="sxs-lookup"><span data-stu-id="3f212-111">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="3f212-112">获取用户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="3f212-112">Get a user's presence information.</span></span>
| [<span data-ttu-id="3f212-113">获取多个用户的状态</span><span class="sxs-lookup"><span data-stu-id="3f212-113">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="3f212-114">[状态](../resources/presence.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f212-114">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="3f212-115">获取多个用户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="3f212-115">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="3f212-116">属性</span><span class="sxs-lookup"><span data-stu-id="3f212-116">Properties</span></span>

| <span data-ttu-id="3f212-117">关系</span><span class="sxs-lookup"><span data-stu-id="3f212-117">Relationship</span></span>        | <span data-ttu-id="3f212-118">类型</span><span class="sxs-lookup"><span data-stu-id="3f212-118">Type</span></span>                                                 | <span data-ttu-id="3f212-119">说明</span><span class="sxs-lookup"><span data-stu-id="3f212-119">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="3f212-120">id</span><span class="sxs-lookup"><span data-stu-id="3f212-120">id</span></span>    |  <span data-ttu-id="3f212-121">string</span><span class="sxs-lookup"><span data-stu-id="3f212-121">string</span></span>     |  <span data-ttu-id="3f212-122">User 对象 id</span><span class="sxs-lookup"><span data-stu-id="3f212-122">The user object id</span></span>   |
|<span data-ttu-id="3f212-123">availability</span><span class="sxs-lookup"><span data-stu-id="3f212-123">availability</span></span>    |  <span data-ttu-id="3f212-124">字符串集合</span><span class="sxs-lookup"><span data-stu-id="3f212-124">string collection</span></span>   |   <span data-ttu-id="3f212-125">用户的基本状态信息。</span><span class="sxs-lookup"><span data-stu-id="3f212-125">The base presence information for a user.</span></span> <span data-ttu-id="3f212-126">可能的值`Available`为`AvailableIdle`、 `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb`、、、、 `Offline`、、`PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="3f212-126">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="3f212-127">activity</span><span class="sxs-lookup"><span data-stu-id="3f212-127">activity</span></span>    |  <span data-ttu-id="3f212-128">字符串集合</span><span class="sxs-lookup"><span data-stu-id="3f212-128">string collection</span></span>      |    <span data-ttu-id="3f212-129">将补充信息提供给用户的可用性。</span><span class="sxs-lookup"><span data-stu-id="3f212-129">The supplemental information to a user's availability.</span></span> <span data-ttu-id="3f212-130">可能的值`Available`为`Away`、 `BeRightBack``Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `UrgentInterruptionsOnly`、、`InAMeeting`、、、、、、、、、、、。 `Offline` `OffWork``OutOfOffice` `PresenceUnknown``Presenting`</span><span class="sxs-lookup"><span data-stu-id="3f212-130">Possible values are `Available`, `Away`, `BeRightBack`,`Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="3f212-131">**注意：** 若要了解有关不同状态的详细信息，请参阅[团队中的用户状态](https://docs.microsoft.com/microsoftteams/presence-admins)。</span><span class="sxs-lookup"><span data-stu-id="3f212-131">**Note:** To learn more about the different presence states, see [User presence in Teams](https://docs.microsoft.com/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="3f212-132">关系</span><span class="sxs-lookup"><span data-stu-id="3f212-132">Relationships</span></span>

<span data-ttu-id="3f212-133">无。</span><span class="sxs-lookup"><span data-stu-id="3f212-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f212-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f212-134">JSON representation</span></span>

<span data-ttu-id="3f212-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f212-135">The following is a JSON representation of the resource.</span></span>

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

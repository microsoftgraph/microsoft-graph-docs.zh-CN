---
title: 状态资源类型
description: 包含有关用户状态的信息，包括其可用性和用户活动。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 257167fe5b7d417751771650f8e5f03b3dd66296
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107688"
---
# <a name="presence-resource-type"></a><span data-ttu-id="83b56-103">状态资源类型</span><span class="sxs-lookup"><span data-stu-id="83b56-103">presence resource type</span></span>

<span data-ttu-id="83b56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83b56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83b56-105">包含有关用户状态的信息，包括其可用性和用户活动。</span><span class="sxs-lookup"><span data-stu-id="83b56-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="83b56-106">**注意：** 此资源当前仅受 Microsoft Teams支持。</span><span class="sxs-lookup"><span data-stu-id="83b56-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="83b56-107">此资源支持订阅 [更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="83b56-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="83b56-108">方法</span><span class="sxs-lookup"><span data-stu-id="83b56-108">Methods</span></span>

| <span data-ttu-id="83b56-109">方法</span><span class="sxs-lookup"><span data-stu-id="83b56-109">Method</span></span>                                                                               | <span data-ttu-id="83b56-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="83b56-110">Return Type</span></span>                                     | <span data-ttu-id="83b56-111">说明</span><span class="sxs-lookup"><span data-stu-id="83b56-111">Description</span></span>                                      |
| :----------------------------------------------------------------------------------- | :---------------------------------------------- | :----------------------------------------------- |
| [<span data-ttu-id="83b56-112">获取状态</span><span class="sxs-lookup"><span data-stu-id="83b56-112">Get presence</span></span>](../api/presence-get.md)                                               | [<span data-ttu-id="83b56-113">状态</span><span class="sxs-lookup"><span data-stu-id="83b56-113">presence</span></span>](../resources/presence.md)            | <span data-ttu-id="83b56-114">获取用户状态信息。</span><span class="sxs-lookup"><span data-stu-id="83b56-114">Get a user's presence information.</span></span>               |
| [<span data-ttu-id="83b56-115">获取多个用户状态</span><span class="sxs-lookup"><span data-stu-id="83b56-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md) | <span data-ttu-id="83b56-116">[presence](../resources/presence.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83b56-116">[presence](../resources/presence.md) collection</span></span> | <span data-ttu-id="83b56-117">获取多个用户状态信息。</span><span class="sxs-lookup"><span data-stu-id="83b56-117">Get the presence information for multiple users.</span></span> |
| [<span data-ttu-id="83b56-118">设置状态</span><span class="sxs-lookup"><span data-stu-id="83b56-118">Set presence</span></span>](../api/presence-setpresence.md)                                               |                                                 | <span data-ttu-id="83b56-119">为用户设置应用程序状态会话。</span><span class="sxs-lookup"><span data-stu-id="83b56-119">Set an application's presence session for a user.</span></span>           |
| [<span data-ttu-id="83b56-120">清除状态</span><span class="sxs-lookup"><span data-stu-id="83b56-120">Clear presence</span></span>](../api/presence-clearpresence.md)                                           |                                                 | <span data-ttu-id="83b56-121">清除用户的应用程序状态会话。</span><span class="sxs-lookup"><span data-stu-id="83b56-121">Clear an application's presence session for a user.</span></span>         |

## <a name="properties"></a><span data-ttu-id="83b56-122">属性</span><span class="sxs-lookup"><span data-stu-id="83b56-122">Properties</span></span>

| <span data-ttu-id="83b56-123">关系</span><span class="sxs-lookup"><span data-stu-id="83b56-123">Relationship</span></span>        | <span data-ttu-id="83b56-124">类型</span><span class="sxs-lookup"><span data-stu-id="83b56-124">Type</span></span>                                          | <span data-ttu-id="83b56-125">说明</span><span class="sxs-lookup"><span data-stu-id="83b56-125">Description</span></span>                                                                                                                                                                                                                                                                                    |
| :------------------ | :-------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="83b56-126">id</span><span class="sxs-lookup"><span data-stu-id="83b56-126">id</span></span>                  | <span data-ttu-id="83b56-127">string</span><span class="sxs-lookup"><span data-stu-id="83b56-127">string</span></span>                                        | <span data-ttu-id="83b56-128">用户对象 ID</span><span class="sxs-lookup"><span data-stu-id="83b56-128">The user object id</span></span>                                                                                                                                                                                                                                                                             |
| <span data-ttu-id="83b56-129">availability</span><span class="sxs-lookup"><span data-stu-id="83b56-129">availability</span></span>        | <span data-ttu-id="83b56-130">string 集合</span><span class="sxs-lookup"><span data-stu-id="83b56-130">string collection</span></span>                             | <span data-ttu-id="83b56-131">用户的基本状态信息。</span><span class="sxs-lookup"><span data-stu-id="83b56-131">The base presence information for a user.</span></span> <span data-ttu-id="83b56-132">可能的值为 `Available` `AvailableIdle` `Away` `BeRightBack` 、、、、、、、、、 `Busy` `BusyIdle` `DoNotDisturb` `Offline``PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="83b56-132">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>                                                                                                           |
| <span data-ttu-id="83b56-133">活动</span><span class="sxs-lookup"><span data-stu-id="83b56-133">activity</span></span>            | <span data-ttu-id="83b56-134">string 集合</span><span class="sxs-lookup"><span data-stu-id="83b56-134">string collection</span></span>                             | <span data-ttu-id="83b56-135">用户可用性的补充信息。</span><span class="sxs-lookup"><span data-stu-id="83b56-135">The supplemental information to a user's availability.</span></span> <span data-ttu-id="83b56-136">可能的值是 `Available` `Away` `BeRightBack` `Busy` 、、、、、、、、、 `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` 。</span><span class="sxs-lookup"><span data-stu-id="83b56-136">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span> |
| <span data-ttu-id="83b56-137">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="83b56-137">outOfOfficeSettings</span></span> | [<span data-ttu-id="83b56-138">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="83b56-138">outOfOfficeSettings</span></span>](outOfOfficeSettings.md) | <span data-ttu-id="83b56-139">用户的外出设置。</span><span class="sxs-lookup"><span data-stu-id="83b56-139">The out of office settings for a user.</span></span>                                                                                                                                                                                                                                                         |

><span data-ttu-id="83b56-140">**注意：** 若要详细了解不同的状态，请参阅用户状态 [Teams。](/microsoftteams/presence-admins)</span><span class="sxs-lookup"><span data-stu-id="83b56-140">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="83b56-141">关系</span><span class="sxs-lookup"><span data-stu-id="83b56-141">Relationships</span></span>

<span data-ttu-id="83b56-142">无。</span><span class="sxs-lookup"><span data-stu-id="83b56-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="83b56-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83b56-143">JSON representation</span></span>

<span data-ttu-id="83b56-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83b56-144">The following is a JSON representation of the resource.</span></span>

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

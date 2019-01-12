---
title: deviceConfigurationTargetedUserAndDevice 资源类型
description: 冲突一设备配置策略的摘要。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 234cc9c909875d835ba54709f30f1ca306eb0954
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947962"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="0c048-103">deviceConfigurationTargetedUserAndDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c048-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="0c048-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0c048-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c048-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0c048-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c048-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0c048-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c048-107">冲突一设备配置策略的摘要。</span><span class="sxs-lookup"><span data-stu-id="0c048-107">Conflict summary for a set of device configuration policies.</span></span>
## <a name="properties"></a><span data-ttu-id="0c048-108">属性</span><span class="sxs-lookup"><span data-stu-id="0c048-108">Properties</span></span>
|<span data-ttu-id="0c048-109">属性</span><span class="sxs-lookup"><span data-stu-id="0c048-109">Property</span></span>|<span data-ttu-id="0c048-110">类型</span><span class="sxs-lookup"><span data-stu-id="0c048-110">Type</span></span>|<span data-ttu-id="0c048-111">说明</span><span class="sxs-lookup"><span data-stu-id="0c048-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c048-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="0c048-112">deviceId</span></span>|<span data-ttu-id="0c048-113">String</span><span class="sxs-lookup"><span data-stu-id="0c048-113">String</span></span>|<span data-ttu-id="0c048-114">签入中的设备 id。</span><span class="sxs-lookup"><span data-stu-id="0c048-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="0c048-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="0c048-115">deviceName</span></span>|<span data-ttu-id="0c048-116">String</span><span class="sxs-lookup"><span data-stu-id="0c048-116">String</span></span>|<span data-ttu-id="0c048-117">签入中的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="0c048-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="0c048-118">userId</span><span class="sxs-lookup"><span data-stu-id="0c048-118">userId</span></span>|<span data-ttu-id="0c048-119">String</span><span class="sxs-lookup"><span data-stu-id="0c048-119">String</span></span>|<span data-ttu-id="0c048-120">在签入的用户 id。</span><span class="sxs-lookup"><span data-stu-id="0c048-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="0c048-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0c048-121">userDisplayName</span></span>|<span data-ttu-id="0c048-122">String</span><span class="sxs-lookup"><span data-stu-id="0c048-122">String</span></span>|<span data-ttu-id="0c048-123">在签入的用户的显示名称</span><span class="sxs-lookup"><span data-stu-id="0c048-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="0c048-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0c048-124">userPrincipalName</span></span>|<span data-ttu-id="0c048-125">字符串</span><span class="sxs-lookup"><span data-stu-id="0c048-125">String</span></span>|<span data-ttu-id="0c048-126">在签入用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="0c048-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="0c048-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="0c048-127">lastCheckinDateTime</span></span>|<span data-ttu-id="0c048-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c048-128">DateTimeOffset</span></span>|<span data-ttu-id="0c048-129">此用户/设备对上一次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="0c048-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c048-130">Relationships</span><span class="sxs-lookup"><span data-stu-id="0c048-130">Relationships</span></span>
<span data-ttu-id="0c048-131">无</span><span class="sxs-lookup"><span data-stu-id="0c048-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c048-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c048-132">JSON Representation</span></span>
<span data-ttu-id="0c048-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c048-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```






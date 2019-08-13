---
title: deviceConfigurationTargetedUserAndDevice 资源类型
description: 一组设备配置策略的冲突摘要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d994491b86d1590c5765d5771ea52b24d6e42f8b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332930"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="551e5-103">deviceConfigurationTargetedUserAndDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="551e5-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="551e5-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="551e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="551e5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="551e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="551e5-106">一组设备配置策略的冲突摘要。</span><span class="sxs-lookup"><span data-stu-id="551e5-106">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="551e5-107">属性</span><span class="sxs-lookup"><span data-stu-id="551e5-107">Properties</span></span>
|<span data-ttu-id="551e5-108">属性</span><span class="sxs-lookup"><span data-stu-id="551e5-108">Property</span></span>|<span data-ttu-id="551e5-109">类型</span><span class="sxs-lookup"><span data-stu-id="551e5-109">Type</span></span>|<span data-ttu-id="551e5-110">说明</span><span class="sxs-lookup"><span data-stu-id="551e5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="551e5-111">deviceId</span><span class="sxs-lookup"><span data-stu-id="551e5-111">deviceId</span></span>|<span data-ttu-id="551e5-112">String</span><span class="sxs-lookup"><span data-stu-id="551e5-112">String</span></span>|<span data-ttu-id="551e5-113">签入中设备的 id。</span><span class="sxs-lookup"><span data-stu-id="551e5-113">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="551e5-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="551e5-114">deviceName</span></span>|<span data-ttu-id="551e5-115">String</span><span class="sxs-lookup"><span data-stu-id="551e5-115">String</span></span>|<span data-ttu-id="551e5-116">签入中设备的名称。</span><span class="sxs-lookup"><span data-stu-id="551e5-116">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="551e5-117">userId</span><span class="sxs-lookup"><span data-stu-id="551e5-117">userId</span></span>|<span data-ttu-id="551e5-118">String</span><span class="sxs-lookup"><span data-stu-id="551e5-118">String</span></span>|<span data-ttu-id="551e5-119">签入中用户的 id。</span><span class="sxs-lookup"><span data-stu-id="551e5-119">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="551e5-120">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="551e5-120">userDisplayName</span></span>|<span data-ttu-id="551e5-121">String</span><span class="sxs-lookup"><span data-stu-id="551e5-121">String</span></span>|<span data-ttu-id="551e5-122">签入用户的显示名称</span><span class="sxs-lookup"><span data-stu-id="551e5-122">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="551e5-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="551e5-123">userPrincipalName</span></span>|<span data-ttu-id="551e5-124">字符串</span><span class="sxs-lookup"><span data-stu-id="551e5-124">String</span></span>|<span data-ttu-id="551e5-125">签入中的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="551e5-125">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="551e5-126">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="551e5-126">lastCheckinDateTime</span></span>|<span data-ttu-id="551e5-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="551e5-127">DateTimeOffset</span></span>|<span data-ttu-id="551e5-128">此用户/设备对的上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="551e5-128">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="551e5-129">关系</span><span class="sxs-lookup"><span data-stu-id="551e5-129">Relationships</span></span>
<span data-ttu-id="551e5-130">无</span><span class="sxs-lookup"><span data-stu-id="551e5-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="551e5-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="551e5-131">JSON Representation</span></span>
<span data-ttu-id="551e5-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="551e5-132">Here is a JSON representation of the resource.</span></span>
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




---
title: deviceConfigurationTargetedUserAndDevice 资源类型
description: 一组设备配置策略的冲突摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c722cf1a21e46ec6066efc1e836793d77ce8e8b7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199390"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="95792-103">deviceConfigurationTargetedUserAndDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="95792-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

<span data-ttu-id="95792-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95792-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95792-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95792-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95792-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95792-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95792-107">一组设备配置策略的冲突摘要。</span><span class="sxs-lookup"><span data-stu-id="95792-107">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="95792-108">属性</span><span class="sxs-lookup"><span data-stu-id="95792-108">Properties</span></span>
|<span data-ttu-id="95792-109">属性</span><span class="sxs-lookup"><span data-stu-id="95792-109">Property</span></span>|<span data-ttu-id="95792-110">类型</span><span class="sxs-lookup"><span data-stu-id="95792-110">Type</span></span>|<span data-ttu-id="95792-111">说明</span><span class="sxs-lookup"><span data-stu-id="95792-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95792-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="95792-112">deviceId</span></span>|<span data-ttu-id="95792-113">String</span><span class="sxs-lookup"><span data-stu-id="95792-113">String</span></span>|<span data-ttu-id="95792-114">签入中设备的 id。</span><span class="sxs-lookup"><span data-stu-id="95792-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="95792-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="95792-115">deviceName</span></span>|<span data-ttu-id="95792-116">String</span><span class="sxs-lookup"><span data-stu-id="95792-116">String</span></span>|<span data-ttu-id="95792-117">签入中设备的名称。</span><span class="sxs-lookup"><span data-stu-id="95792-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="95792-118">userId</span><span class="sxs-lookup"><span data-stu-id="95792-118">userId</span></span>|<span data-ttu-id="95792-119">String</span><span class="sxs-lookup"><span data-stu-id="95792-119">String</span></span>|<span data-ttu-id="95792-120">签入中用户的 id。</span><span class="sxs-lookup"><span data-stu-id="95792-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="95792-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="95792-121">userDisplayName</span></span>|<span data-ttu-id="95792-122">String</span><span class="sxs-lookup"><span data-stu-id="95792-122">String</span></span>|<span data-ttu-id="95792-123">签入用户的显示名称</span><span class="sxs-lookup"><span data-stu-id="95792-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="95792-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="95792-124">userPrincipalName</span></span>|<span data-ttu-id="95792-125">String</span><span class="sxs-lookup"><span data-stu-id="95792-125">String</span></span>|<span data-ttu-id="95792-126">签入中的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="95792-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="95792-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="95792-127">lastCheckinDateTime</span></span>|<span data-ttu-id="95792-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95792-128">DateTimeOffset</span></span>|<span data-ttu-id="95792-129">此用户/设备对的上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="95792-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95792-130">关系</span><span class="sxs-lookup"><span data-stu-id="95792-130">Relationships</span></span>
<span data-ttu-id="95792-131">无</span><span class="sxs-lookup"><span data-stu-id="95792-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95792-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95792-132">JSON Representation</span></span>
<span data-ttu-id="95792-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95792-133">Here is a JSON representation of the resource.</span></span>
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





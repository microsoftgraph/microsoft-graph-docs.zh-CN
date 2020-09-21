---
title: deviceConfigurationTargetedUserAndDevice 资源类型
description: 一组设备配置策略的冲突摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb569346aa16f42c50f8ddb246f127bfeadae087
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016343"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="d7687-103">deviceConfigurationTargetedUserAndDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7687-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

<span data-ttu-id="d7687-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7687-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7687-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d7687-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7687-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d7687-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7687-107">一组设备配置策略的冲突摘要。</span><span class="sxs-lookup"><span data-stu-id="d7687-107">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="d7687-108">属性</span><span class="sxs-lookup"><span data-stu-id="d7687-108">Properties</span></span>
|<span data-ttu-id="d7687-109">属性</span><span class="sxs-lookup"><span data-stu-id="d7687-109">Property</span></span>|<span data-ttu-id="d7687-110">类型</span><span class="sxs-lookup"><span data-stu-id="d7687-110">Type</span></span>|<span data-ttu-id="d7687-111">说明</span><span class="sxs-lookup"><span data-stu-id="d7687-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7687-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="d7687-112">deviceId</span></span>|<span data-ttu-id="d7687-113">String</span><span class="sxs-lookup"><span data-stu-id="d7687-113">String</span></span>|<span data-ttu-id="d7687-114">签入中设备的 id。</span><span class="sxs-lookup"><span data-stu-id="d7687-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="d7687-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="d7687-115">deviceName</span></span>|<span data-ttu-id="d7687-116">String</span><span class="sxs-lookup"><span data-stu-id="d7687-116">String</span></span>|<span data-ttu-id="d7687-117">签入中设备的名称。</span><span class="sxs-lookup"><span data-stu-id="d7687-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="d7687-118">userId</span><span class="sxs-lookup"><span data-stu-id="d7687-118">userId</span></span>|<span data-ttu-id="d7687-119">String</span><span class="sxs-lookup"><span data-stu-id="d7687-119">String</span></span>|<span data-ttu-id="d7687-120">签入中用户的 id。</span><span class="sxs-lookup"><span data-stu-id="d7687-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="d7687-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d7687-121">userDisplayName</span></span>|<span data-ttu-id="d7687-122">String</span><span class="sxs-lookup"><span data-stu-id="d7687-122">String</span></span>|<span data-ttu-id="d7687-123">签入用户的显示名称</span><span class="sxs-lookup"><span data-stu-id="d7687-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="d7687-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d7687-124">userPrincipalName</span></span>|<span data-ttu-id="d7687-125">String</span><span class="sxs-lookup"><span data-stu-id="d7687-125">String</span></span>|<span data-ttu-id="d7687-126">签入中的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="d7687-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="d7687-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="d7687-127">lastCheckinDateTime</span></span>|<span data-ttu-id="d7687-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7687-128">DateTimeOffset</span></span>|<span data-ttu-id="d7687-129">此用户/设备对的上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="d7687-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7687-130">关系</span><span class="sxs-lookup"><span data-stu-id="d7687-130">Relationships</span></span>
<span data-ttu-id="d7687-131">无</span><span class="sxs-lookup"><span data-stu-id="d7687-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7687-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7687-132">JSON Representation</span></span>
<span data-ttu-id="d7687-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7687-133">Here is a JSON representation of the resource.</span></span>
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







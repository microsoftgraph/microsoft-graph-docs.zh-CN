---
title: deviceConfigurationTargetedUserAndDevice 资源类型
description: 冲突一设备配置策略的摘要。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e246d9731f5ed9d2ea888ba2b53d335fcbca19f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410740"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="faa73-103">deviceConfigurationTargetedUserAndDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="faa73-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="faa73-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="faa73-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="faa73-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="faa73-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="faa73-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="faa73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faa73-107">冲突一设备配置策略的摘要。</span><span class="sxs-lookup"><span data-stu-id="faa73-107">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="faa73-108">属性</span><span class="sxs-lookup"><span data-stu-id="faa73-108">Properties</span></span>
|<span data-ttu-id="faa73-109">属性</span><span class="sxs-lookup"><span data-stu-id="faa73-109">Property</span></span>|<span data-ttu-id="faa73-110">类型</span><span class="sxs-lookup"><span data-stu-id="faa73-110">Type</span></span>|<span data-ttu-id="faa73-111">说明</span><span class="sxs-lookup"><span data-stu-id="faa73-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faa73-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="faa73-112">deviceId</span></span>|<span data-ttu-id="faa73-113">String</span><span class="sxs-lookup"><span data-stu-id="faa73-113">String</span></span>|<span data-ttu-id="faa73-114">签入中的设备 id。</span><span class="sxs-lookup"><span data-stu-id="faa73-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="faa73-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="faa73-115">deviceName</span></span>|<span data-ttu-id="faa73-116">String</span><span class="sxs-lookup"><span data-stu-id="faa73-116">String</span></span>|<span data-ttu-id="faa73-117">签入中的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="faa73-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="faa73-118">userId</span><span class="sxs-lookup"><span data-stu-id="faa73-118">userId</span></span>|<span data-ttu-id="faa73-119">String</span><span class="sxs-lookup"><span data-stu-id="faa73-119">String</span></span>|<span data-ttu-id="faa73-120">在签入的用户 id。</span><span class="sxs-lookup"><span data-stu-id="faa73-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="faa73-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="faa73-121">userDisplayName</span></span>|<span data-ttu-id="faa73-122">String</span><span class="sxs-lookup"><span data-stu-id="faa73-122">String</span></span>|<span data-ttu-id="faa73-123">在签入的用户的显示名称</span><span class="sxs-lookup"><span data-stu-id="faa73-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="faa73-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="faa73-124">userPrincipalName</span></span>|<span data-ttu-id="faa73-125">String</span><span class="sxs-lookup"><span data-stu-id="faa73-125">String</span></span>|<span data-ttu-id="faa73-126">在签入用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="faa73-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="faa73-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="faa73-127">lastCheckinDateTime</span></span>|<span data-ttu-id="faa73-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faa73-128">DateTimeOffset</span></span>|<span data-ttu-id="faa73-129">此用户/设备对上一次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="faa73-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="faa73-130">关系</span><span class="sxs-lookup"><span data-stu-id="faa73-130">Relationships</span></span>
<span data-ttu-id="faa73-131">无</span><span class="sxs-lookup"><span data-stu-id="faa73-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="faa73-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="faa73-132">JSON Representation</span></span>
<span data-ttu-id="faa73-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="faa73-133">Here is a JSON representation of the resource.</span></span>
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





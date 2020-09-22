---
title: officeClientCheckinStatus 资源类型
description: 描述租户签入统计信息的实体。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 647d55e3d5eca6acb47b90092dc0502097b63cf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021761"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="48509-103">officeClientCheckinStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="48509-103">officeClientCheckinStatus resource type</span></span>

<span data-ttu-id="48509-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48509-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48509-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="48509-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48509-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="48509-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48509-107">描述租户签入统计信息的实体。</span><span class="sxs-lookup"><span data-stu-id="48509-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="48509-108">属性</span><span class="sxs-lookup"><span data-stu-id="48509-108">Properties</span></span>
|<span data-ttu-id="48509-109">属性</span><span class="sxs-lookup"><span data-stu-id="48509-109">Property</span></span>|<span data-ttu-id="48509-110">类型</span><span class="sxs-lookup"><span data-stu-id="48509-110">Type</span></span>|<span data-ttu-id="48509-111">说明</span><span class="sxs-lookup"><span data-stu-id="48509-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48509-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="48509-112">userPrincipalName</span></span>|<span data-ttu-id="48509-113">String</span><span class="sxs-lookup"><span data-stu-id="48509-113">String</span></span>|<span data-ttu-id="48509-114">使用设备的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="48509-114">User principal name using the device.</span></span>|
|<span data-ttu-id="48509-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="48509-115">deviceName</span></span>|<span data-ttu-id="48509-116">String</span><span class="sxs-lookup"><span data-stu-id="48509-116">String</span></span>|<span data-ttu-id="48509-117">尝试签入的设备名称。</span><span class="sxs-lookup"><span data-stu-id="48509-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="48509-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="48509-118">devicePlatform</span></span>|<span data-ttu-id="48509-119">String</span><span class="sxs-lookup"><span data-stu-id="48509-119">String</span></span>|<span data-ttu-id="48509-120">尝试签入的设备平台。</span><span class="sxs-lookup"><span data-stu-id="48509-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="48509-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="48509-121">devicePlatformVersion</span></span>|<span data-ttu-id="48509-122">String</span><span class="sxs-lookup"><span data-stu-id="48509-122">String</span></span>|<span data-ttu-id="48509-123">尝试签入的设备平台版本。</span><span class="sxs-lookup"><span data-stu-id="48509-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="48509-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="48509-124">wasSuccessful</span></span>|<span data-ttu-id="48509-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="48509-125">Boolean</span></span>|<span data-ttu-id="48509-126">如果上一次签入成功。</span><span class="sxs-lookup"><span data-stu-id="48509-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="48509-127">userId</span><span class="sxs-lookup"><span data-stu-id="48509-127">userId</span></span>|<span data-ttu-id="48509-128">String</span><span class="sxs-lookup"><span data-stu-id="48509-128">String</span></span>|<span data-ttu-id="48509-129">使用设备的用户标识符。</span><span class="sxs-lookup"><span data-stu-id="48509-129">User identifier using the device.</span></span>|
|<span data-ttu-id="48509-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="48509-130">checkinDateTime</span></span>|<span data-ttu-id="48509-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48509-131">DateTimeOffset</span></span>|<span data-ttu-id="48509-132">UTC 格式的上次设备签入时间。</span><span class="sxs-lookup"><span data-stu-id="48509-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="48509-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="48509-133">errorMessage</span></span>|<span data-ttu-id="48509-134">String</span><span class="sxs-lookup"><span data-stu-id="48509-134">String</span></span>|<span data-ttu-id="48509-135">如果与上次签入相关联，则出现错误消息。</span><span class="sxs-lookup"><span data-stu-id="48509-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="48509-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="48509-136">appliedPolicies</span></span>|<span data-ttu-id="48509-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="48509-137">String collection</span></span>|<span data-ttu-id="48509-138">上次签入到设备的策略列表。</span><span class="sxs-lookup"><span data-stu-id="48509-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48509-139">关系</span><span class="sxs-lookup"><span data-stu-id="48509-139">Relationships</span></span>
<span data-ttu-id="48509-140">无</span><span class="sxs-lookup"><span data-stu-id="48509-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48509-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48509-141">JSON Representation</span></span>
<span data-ttu-id="48509-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48509-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
  "userPrincipalName": "String",
  "deviceName": "String",
  "devicePlatform": "String",
  "devicePlatformVersion": "String",
  "wasSuccessful": true,
  "userId": "String",
  "checkinDateTime": "String (timestamp)",
  "errorMessage": "String",
  "appliedPolicies": [
    "String"
  ]
}
```







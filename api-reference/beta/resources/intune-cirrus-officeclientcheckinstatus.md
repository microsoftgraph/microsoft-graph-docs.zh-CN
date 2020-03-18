---
title: officeClientCheckinStatus 资源类型
description: 描述租户签入统计信息的实体。
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 66087cd47fa70352f8051fc220820ea355805f19
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797337"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="64984-103">officeClientCheckinStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="64984-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="64984-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64984-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64984-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64984-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64984-106">描述租户签入统计信息的实体。</span><span class="sxs-lookup"><span data-stu-id="64984-106">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="64984-107">属性</span><span class="sxs-lookup"><span data-stu-id="64984-107">Properties</span></span>
|<span data-ttu-id="64984-108">属性</span><span class="sxs-lookup"><span data-stu-id="64984-108">Property</span></span>|<span data-ttu-id="64984-109">类型</span><span class="sxs-lookup"><span data-stu-id="64984-109">Type</span></span>|<span data-ttu-id="64984-110">说明</span><span class="sxs-lookup"><span data-stu-id="64984-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64984-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="64984-111">userPrincipalName</span></span>|<span data-ttu-id="64984-112">字符串</span><span class="sxs-lookup"><span data-stu-id="64984-112">String</span></span>|<span data-ttu-id="64984-113">使用设备的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="64984-113">User principal name using the device.</span></span>|
|<span data-ttu-id="64984-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="64984-114">deviceName</span></span>|<span data-ttu-id="64984-115">String</span><span class="sxs-lookup"><span data-stu-id="64984-115">String</span></span>|<span data-ttu-id="64984-116">尝试签入的设备名称。</span><span class="sxs-lookup"><span data-stu-id="64984-116">Device name trying to check-in.</span></span>|
|<span data-ttu-id="64984-117">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="64984-117">devicePlatform</span></span>|<span data-ttu-id="64984-118">String</span><span class="sxs-lookup"><span data-stu-id="64984-118">String</span></span>|<span data-ttu-id="64984-119">尝试签入的设备平台。</span><span class="sxs-lookup"><span data-stu-id="64984-119">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="64984-120">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="64984-120">devicePlatformVersion</span></span>|<span data-ttu-id="64984-121">String</span><span class="sxs-lookup"><span data-stu-id="64984-121">String</span></span>|<span data-ttu-id="64984-122">尝试签入的设备平台版本。</span><span class="sxs-lookup"><span data-stu-id="64984-122">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="64984-123">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="64984-123">wasSuccessful</span></span>|<span data-ttu-id="64984-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="64984-124">Boolean</span></span>|<span data-ttu-id="64984-125">如果上一次签入成功。</span><span class="sxs-lookup"><span data-stu-id="64984-125">If the last checkin was successful.</span></span>|
|<span data-ttu-id="64984-126">userId</span><span class="sxs-lookup"><span data-stu-id="64984-126">userId</span></span>|<span data-ttu-id="64984-127">String</span><span class="sxs-lookup"><span data-stu-id="64984-127">String</span></span>|<span data-ttu-id="64984-128">使用设备的用户标识符。</span><span class="sxs-lookup"><span data-stu-id="64984-128">User identifier using the device.</span></span>|
|<span data-ttu-id="64984-129">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="64984-129">checkinDateTime</span></span>|<span data-ttu-id="64984-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64984-130">DateTimeOffset</span></span>|<span data-ttu-id="64984-131">UTC 格式的上次设备签入时间。</span><span class="sxs-lookup"><span data-stu-id="64984-131">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="64984-132">errorMessage</span><span class="sxs-lookup"><span data-stu-id="64984-132">errorMessage</span></span>|<span data-ttu-id="64984-133">String</span><span class="sxs-lookup"><span data-stu-id="64984-133">String</span></span>|<span data-ttu-id="64984-134">如果与上次签入相关联，则出现错误消息。</span><span class="sxs-lookup"><span data-stu-id="64984-134">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="64984-135">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="64984-135">appliedPolicies</span></span>|<span data-ttu-id="64984-136">String collection</span><span class="sxs-lookup"><span data-stu-id="64984-136">String collection</span></span>|<span data-ttu-id="64984-137">上次签入到设备的策略列表。</span><span class="sxs-lookup"><span data-stu-id="64984-137">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64984-138">关系</span><span class="sxs-lookup"><span data-stu-id="64984-138">Relationships</span></span>
<span data-ttu-id="64984-139">无</span><span class="sxs-lookup"><span data-stu-id="64984-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64984-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64984-140">JSON Representation</span></span>
<span data-ttu-id="64984-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64984-141">Here is a JSON representation of the resource.</span></span>
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




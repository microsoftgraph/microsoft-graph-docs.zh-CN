---
title: officeClientCheckinStatus 资源类型
description: 介绍租户中签入 stats 的实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aebc534a6c424a9dac4316d0029e2fd35839f0a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403257"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="7ce48-103">officeClientCheckinStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ce48-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="7ce48-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7ce48-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7ce48-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7ce48-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ce48-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ce48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ce48-107">介绍租户中签入 stats 的实体。</span><span class="sxs-lookup"><span data-stu-id="7ce48-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="7ce48-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ce48-108">Properties</span></span>
|<span data-ttu-id="7ce48-109">属性</span><span class="sxs-lookup"><span data-stu-id="7ce48-109">Property</span></span>|<span data-ttu-id="7ce48-110">类型</span><span class="sxs-lookup"><span data-stu-id="7ce48-110">Type</span></span>|<span data-ttu-id="7ce48-111">说明</span><span class="sxs-lookup"><span data-stu-id="7ce48-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ce48-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7ce48-112">userPrincipalName</span></span>|<span data-ttu-id="7ce48-113">String</span><span class="sxs-lookup"><span data-stu-id="7ce48-113">String</span></span>|<span data-ttu-id="7ce48-114">使用设备的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="7ce48-114">User principal name using the device.</span></span>|
|<span data-ttu-id="7ce48-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="7ce48-115">deviceName</span></span>|<span data-ttu-id="7ce48-116">String</span><span class="sxs-lookup"><span data-stu-id="7ce48-116">String</span></span>|<span data-ttu-id="7ce48-117">要签入的设备名称。</span><span class="sxs-lookup"><span data-stu-id="7ce48-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="7ce48-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="7ce48-118">devicePlatform</span></span>|<span data-ttu-id="7ce48-119">String</span><span class="sxs-lookup"><span data-stu-id="7ce48-119">String</span></span>|<span data-ttu-id="7ce48-120">要签入的设备平台。</span><span class="sxs-lookup"><span data-stu-id="7ce48-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="7ce48-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="7ce48-121">devicePlatformVersion</span></span>|<span data-ttu-id="7ce48-122">String</span><span class="sxs-lookup"><span data-stu-id="7ce48-122">String</span></span>|<span data-ttu-id="7ce48-123">要签入的设备平台版本。</span><span class="sxs-lookup"><span data-stu-id="7ce48-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="7ce48-124">准备成功</span><span class="sxs-lookup"><span data-stu-id="7ce48-124">wasSuccessful</span></span>|<span data-ttu-id="7ce48-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ce48-125">Boolean</span></span>|<span data-ttu-id="7ce48-126">如果上次签入已成功。</span><span class="sxs-lookup"><span data-stu-id="7ce48-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="7ce48-127">userId</span><span class="sxs-lookup"><span data-stu-id="7ce48-127">userId</span></span>|<span data-ttu-id="7ce48-128">String</span><span class="sxs-lookup"><span data-stu-id="7ce48-128">String</span></span>|<span data-ttu-id="7ce48-129">使用设备的用户标识符。</span><span class="sxs-lookup"><span data-stu-id="7ce48-129">User identifier using the device.</span></span>|
|<span data-ttu-id="7ce48-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="7ce48-130">checkinDateTime</span></span>|<span data-ttu-id="7ce48-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ce48-131">DateTimeOffset</span></span>|<span data-ttu-id="7ce48-132">最后一个设备签入时间采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="7ce48-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="7ce48-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="7ce48-133">errorMessage</span></span>|<span data-ttu-id="7ce48-134">String</span><span class="sxs-lookup"><span data-stu-id="7ce48-134">String</span></span>|<span data-ttu-id="7ce48-135">如果有关联的最后一个签入的错误消息。</span><span class="sxs-lookup"><span data-stu-id="7ce48-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="7ce48-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="7ce48-136">appliedPolicies</span></span>|<span data-ttu-id="7ce48-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="7ce48-137">String collection</span></span>|<span data-ttu-id="7ce48-138">策略列表送达作为最后一个签入的设备。</span><span class="sxs-lookup"><span data-stu-id="7ce48-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ce48-139">关系</span><span class="sxs-lookup"><span data-stu-id="7ce48-139">Relationships</span></span>
<span data-ttu-id="7ce48-140">无</span><span class="sxs-lookup"><span data-stu-id="7ce48-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ce48-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ce48-141">JSON Representation</span></span>
<span data-ttu-id="7ce48-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ce48-142">Here is a JSON representation of the resource.</span></span>
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




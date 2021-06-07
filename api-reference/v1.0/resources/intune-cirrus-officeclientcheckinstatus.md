---
title: officeClientCheckinStatus 资源类型
description: 描述租户签入统计数据的实体。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bdd2d4f47244bb2eab1e7c357a9f599909166b6a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758523"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="ed77c-103">officeClientCheckinStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed77c-103">officeClientCheckinStatus resource type</span></span>

<span data-ttu-id="ed77c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed77c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed77c-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ed77c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed77c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed77c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed77c-107">描述租户签入统计数据的实体。</span><span class="sxs-lookup"><span data-stu-id="ed77c-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="ed77c-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed77c-108">Properties</span></span>
|<span data-ttu-id="ed77c-109">属性</span><span class="sxs-lookup"><span data-stu-id="ed77c-109">Property</span></span>|<span data-ttu-id="ed77c-110">类型</span><span class="sxs-lookup"><span data-stu-id="ed77c-110">Type</span></span>|<span data-ttu-id="ed77c-111">说明</span><span class="sxs-lookup"><span data-stu-id="ed77c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed77c-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ed77c-112">userPrincipalName</span></span>|<span data-ttu-id="ed77c-113">String</span><span class="sxs-lookup"><span data-stu-id="ed77c-113">String</span></span>|<span data-ttu-id="ed77c-114">使用设备的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="ed77c-114">User principal name using the device.</span></span>|
|<span data-ttu-id="ed77c-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="ed77c-115">deviceName</span></span>|<span data-ttu-id="ed77c-116">String</span><span class="sxs-lookup"><span data-stu-id="ed77c-116">String</span></span>|<span data-ttu-id="ed77c-117">尝试签入的设备名称。</span><span class="sxs-lookup"><span data-stu-id="ed77c-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="ed77c-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="ed77c-118">devicePlatform</span></span>|<span data-ttu-id="ed77c-119">String</span><span class="sxs-lookup"><span data-stu-id="ed77c-119">String</span></span>|<span data-ttu-id="ed77c-120">尝试签入的设备平台。</span><span class="sxs-lookup"><span data-stu-id="ed77c-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="ed77c-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="ed77c-121">devicePlatformVersion</span></span>|<span data-ttu-id="ed77c-122">String</span><span class="sxs-lookup"><span data-stu-id="ed77c-122">String</span></span>|<span data-ttu-id="ed77c-123">尝试签入的设备平台版本。</span><span class="sxs-lookup"><span data-stu-id="ed77c-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="ed77c-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="ed77c-124">wasSuccessful</span></span>|<span data-ttu-id="ed77c-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed77c-125">Boolean</span></span>|<span data-ttu-id="ed77c-126">如果最后一次签入成功。</span><span class="sxs-lookup"><span data-stu-id="ed77c-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="ed77c-127">userId</span><span class="sxs-lookup"><span data-stu-id="ed77c-127">userId</span></span>|<span data-ttu-id="ed77c-128">String</span><span class="sxs-lookup"><span data-stu-id="ed77c-128">String</span></span>|<span data-ttu-id="ed77c-129">使用设备的用户标识符。</span><span class="sxs-lookup"><span data-stu-id="ed77c-129">User identifier using the device.</span></span>|
|<span data-ttu-id="ed77c-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="ed77c-130">checkinDateTime</span></span>|<span data-ttu-id="ed77c-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed77c-131">DateTimeOffset</span></span>|<span data-ttu-id="ed77c-132">上次设备签入时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="ed77c-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="ed77c-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="ed77c-133">errorMessage</span></span>|<span data-ttu-id="ed77c-134">String</span><span class="sxs-lookup"><span data-stu-id="ed77c-134">String</span></span>|<span data-ttu-id="ed77c-135">错误消息（如果与最后一个签入有任何关联）。</span><span class="sxs-lookup"><span data-stu-id="ed77c-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="ed77c-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="ed77c-136">appliedPolicies</span></span>|<span data-ttu-id="ed77c-137">String collection</span><span class="sxs-lookup"><span data-stu-id="ed77c-137">String collection</span></span>|<span data-ttu-id="ed77c-138">作为最后一个签入传递到设备的策略列表。</span><span class="sxs-lookup"><span data-stu-id="ed77c-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed77c-139">关系</span><span class="sxs-lookup"><span data-stu-id="ed77c-139">Relationships</span></span>
<span data-ttu-id="ed77c-140">无</span><span class="sxs-lookup"><span data-stu-id="ed77c-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed77c-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed77c-141">JSON Representation</span></span>
<span data-ttu-id="ed77c-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed77c-142">Here is a JSON representation of the resource.</span></span>
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





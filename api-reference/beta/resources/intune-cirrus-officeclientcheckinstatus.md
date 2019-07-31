---
title: officeClientCheckinStatus 资源类型
description: 描述租户签入统计信息的实体。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df8f1927329a34a51b5f6d8738faec05be01b451
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012000"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="b6fa5-103">officeClientCheckinStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6fa5-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="b6fa5-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b6fa5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6fa5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6fa5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6fa5-106">描述租户签入统计信息的实体。</span><span class="sxs-lookup"><span data-stu-id="b6fa5-106">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="b6fa5-107">属性</span><span class="sxs-lookup"><span data-stu-id="b6fa5-107">Properties</span></span>
|<span data-ttu-id="b6fa5-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6fa5-108">Property</span></span>|<span data-ttu-id="b6fa5-109">类型</span><span class="sxs-lookup"><span data-stu-id="b6fa5-109">Type</span></span>|<span data-ttu-id="b6fa5-110">说明</span><span class="sxs-lookup"><span data-stu-id="b6fa5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6fa5-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b6fa5-111">userPrincipalName</span></span>|<span data-ttu-id="b6fa5-112">字符串</span><span class="sxs-lookup"><span data-stu-id="b6fa5-112">String</span></span>|<span data-ttu-id="b6fa5-113">使用设备的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="b6fa5-113">User principal name using the device.</span></span>|
|<span data-ttu-id="b6fa5-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="b6fa5-114">deviceName</span></span>|<span data-ttu-id="b6fa5-115">String</span><span class="sxs-lookup"><span data-stu-id="b6fa5-115">String</span></span>|<span data-ttu-id="b6fa5-116">尝试签入的设备名称。</span><span class="sxs-lookup"><span data-stu-id="b6fa5-116">Device name trying to check-in.</span></span>|
|<span data-ttu-id="b6fa5-117">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="b6fa5-117">devicePlatform</span></span>|<span data-ttu-id="b6fa5-118">String</span><span class="sxs-lookup"><span data-stu-id="b6fa5-118">String</span></span>|<span data-ttu-id="b6fa5-119">尝试签入的设备平台。</span><span class="sxs-lookup"><span data-stu-id="b6fa5-119">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="b6fa5-120">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="b6fa5-120">devicePlatformVersion</span></span>|<span data-ttu-id="b6fa5-121">String</span><span class="sxs-lookup"><span data-stu-id="b6fa5-121">String</span></span>|<span data-ttu-id="b6fa5-122">尝试签入的设备平台版本。</span><span class="sxs-lookup"><span data-stu-id="b6fa5-122">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="b6fa5-123">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="b6fa5-123">wasSuccessful</span></span>|<span data-ttu-id="b6fa5-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6fa5-124">Boolean</span></span>|<span data-ttu-id="b6fa5-125">如果上一次签入成功。</span><span class="sxs-lookup"><span data-stu-id="b6fa5-125">If the last checkin was successful.</span></span>|
|<span data-ttu-id="b6fa5-126">userId</span><span class="sxs-lookup"><span data-stu-id="b6fa5-126">userId</span></span>|<span data-ttu-id="b6fa5-127">String</span><span class="sxs-lookup"><span data-stu-id="b6fa5-127">String</span></span>|<span data-ttu-id="b6fa5-128">使用设备的用户标识符。</span><span class="sxs-lookup"><span data-stu-id="b6fa5-128">User identifier using the device.</span></span>|
|<span data-ttu-id="b6fa5-129">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="b6fa5-129">checkinDateTime</span></span>|<span data-ttu-id="b6fa5-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6fa5-130">DateTimeOffset</span></span>|<span data-ttu-id="b6fa5-131">UTC 格式的上次设备签入时间。</span><span class="sxs-lookup"><span data-stu-id="b6fa5-131">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="b6fa5-132">errorMessage</span><span class="sxs-lookup"><span data-stu-id="b6fa5-132">errorMessage</span></span>|<span data-ttu-id="b6fa5-133">String</span><span class="sxs-lookup"><span data-stu-id="b6fa5-133">String</span></span>|<span data-ttu-id="b6fa5-134">如果与上次签入相关联, 则出现错误消息。</span><span class="sxs-lookup"><span data-stu-id="b6fa5-134">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="b6fa5-135">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="b6fa5-135">appliedPolicies</span></span>|<span data-ttu-id="b6fa5-136">String collection</span><span class="sxs-lookup"><span data-stu-id="b6fa5-136">String collection</span></span>|<span data-ttu-id="b6fa5-137">上次签入到设备的策略列表。</span><span class="sxs-lookup"><span data-stu-id="b6fa5-137">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6fa5-138">关系</span><span class="sxs-lookup"><span data-stu-id="b6fa5-138">Relationships</span></span>
<span data-ttu-id="b6fa5-139">无</span><span class="sxs-lookup"><span data-stu-id="b6fa5-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6fa5-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6fa5-140">JSON Representation</span></span>
<span data-ttu-id="b6fa5-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6fa5-141">Here is a JSON representation of the resource.</span></span>
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




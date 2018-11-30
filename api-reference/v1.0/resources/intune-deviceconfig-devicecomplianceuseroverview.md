---
title: deviceComplianceUserOverview 资源类型
description: 尚未记录
ms.openlocfilehash: a650d9e017bbcca825aa7f15f829bba572f7e48f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009310"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="ce977-103">deviceComplianceUserOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce977-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="ce977-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ce977-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce977-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ce977-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="ce977-106">方法</span><span class="sxs-lookup"><span data-stu-id="ce977-106">Methods</span></span>
|<span data-ttu-id="ce977-107">方法</span><span class="sxs-lookup"><span data-stu-id="ce977-107">Method</span></span>|<span data-ttu-id="ce977-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ce977-108">Return Type</span></span>|<span data-ttu-id="ce977-109">说明</span><span class="sxs-lookup"><span data-stu-id="ce977-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ce977-110">获取 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="ce977-110">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="ce977-111">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="ce977-111">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="ce977-112">读取 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ce977-112">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="ce977-113">更新 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="ce977-113">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="ce977-114">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="ce977-114">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="ce977-115">更新 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ce977-115">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ce977-116">属性</span><span class="sxs-lookup"><span data-stu-id="ce977-116">Properties</span></span>
|<span data-ttu-id="ce977-117">属性</span><span class="sxs-lookup"><span data-stu-id="ce977-117">Property</span></span>|<span data-ttu-id="ce977-118">类型</span><span class="sxs-lookup"><span data-stu-id="ce977-118">Type</span></span>|<span data-ttu-id="ce977-119">说明</span><span class="sxs-lookup"><span data-stu-id="ce977-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce977-120">id</span><span class="sxs-lookup"><span data-stu-id="ce977-120">id</span></span>|<span data-ttu-id="ce977-121">String</span><span class="sxs-lookup"><span data-stu-id="ce977-121">String</span></span>|<span data-ttu-id="ce977-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ce977-122">Key of the entity.</span></span>|
|<span data-ttu-id="ce977-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="ce977-123">pendingCount</span></span>|<span data-ttu-id="ce977-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ce977-124">Int32</span></span>|<span data-ttu-id="ce977-125">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="ce977-125">Number of pending Users</span></span>|
|<span data-ttu-id="ce977-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="ce977-126">notApplicableCount</span></span>|<span data-ttu-id="ce977-127">Int32</span><span class="sxs-lookup"><span data-stu-id="ce977-127">Int32</span></span>|<span data-ttu-id="ce977-128">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="ce977-128">Number of not applicable users</span></span>|
|<span data-ttu-id="ce977-129">successCount</span><span class="sxs-lookup"><span data-stu-id="ce977-129">successCount</span></span>|<span data-ttu-id="ce977-130">Int32</span><span class="sxs-lookup"><span data-stu-id="ce977-130">Int32</span></span>|<span data-ttu-id="ce977-131">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="ce977-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="ce977-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="ce977-132">errorCount</span></span>|<span data-ttu-id="ce977-133">Int32</span><span class="sxs-lookup"><span data-stu-id="ce977-133">Int32</span></span>|<span data-ttu-id="ce977-134">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="ce977-134">Number of error Users</span></span>|
|<span data-ttu-id="ce977-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="ce977-135">failedCount</span></span>|<span data-ttu-id="ce977-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ce977-136">Int32</span></span>|<span data-ttu-id="ce977-137">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="ce977-137">Number of failed Users</span></span>|
|<span data-ttu-id="ce977-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="ce977-138">lastUpdateDateTime</span></span>|<span data-ttu-id="ce977-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce977-139">DateTimeOffset</span></span>|<span data-ttu-id="ce977-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="ce977-140">Last update time</span></span>|
|<span data-ttu-id="ce977-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="ce977-141">configurationVersion</span></span>|<span data-ttu-id="ce977-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ce977-142">Int32</span></span>|<span data-ttu-id="ce977-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="ce977-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce977-144">关系</span><span class="sxs-lookup"><span data-stu-id="ce977-144">Relationships</span></span>
<span data-ttu-id="ce977-145">无</span><span class="sxs-lookup"><span data-stu-id="ce977-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ce977-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce977-146">JSON Representation</span></span>
<span data-ttu-id="ce977-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce977-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```




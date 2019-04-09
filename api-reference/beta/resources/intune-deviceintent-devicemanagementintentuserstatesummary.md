---
title: deviceManagementIntentUserStateSummary 资源类型
description: 表示意向的用户状态摘要的实体
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c930b19e604aaf3867260e359a2b7fcb12153762
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523992"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a><span data-ttu-id="110b7-103">deviceManagementIntentUserStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="110b7-103">deviceManagementIntentUserStateSummary resource type</span></span>

> <span data-ttu-id="110b7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="110b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="110b7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="110b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="110b7-106">表示意向的用户状态摘要的实体</span><span class="sxs-lookup"><span data-stu-id="110b7-106">Entity that represents user state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="110b7-107">方法</span><span class="sxs-lookup"><span data-stu-id="110b7-107">Methods</span></span>
|<span data-ttu-id="110b7-108">方法</span><span class="sxs-lookup"><span data-stu-id="110b7-108">Method</span></span>|<span data-ttu-id="110b7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="110b7-109">Return Type</span></span>|<span data-ttu-id="110b7-110">说明</span><span class="sxs-lookup"><span data-stu-id="110b7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="110b7-111">获取 deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="110b7-111">Get deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[<span data-ttu-id="110b7-112">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="110b7-112">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="110b7-113">读取[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="110b7-113">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="110b7-114">更新 deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="110b7-114">Update deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[<span data-ttu-id="110b7-115">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="110b7-115">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="110b7-116">更新[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="110b7-116">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="110b7-117">属性</span><span class="sxs-lookup"><span data-stu-id="110b7-117">Properties</span></span>
|<span data-ttu-id="110b7-118">属性</span><span class="sxs-lookup"><span data-stu-id="110b7-118">Property</span></span>|<span data-ttu-id="110b7-119">类型</span><span class="sxs-lookup"><span data-stu-id="110b7-119">Type</span></span>|<span data-ttu-id="110b7-120">说明</span><span class="sxs-lookup"><span data-stu-id="110b7-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="110b7-121">id</span><span class="sxs-lookup"><span data-stu-id="110b7-121">id</span></span>|<span data-ttu-id="110b7-122">String</span><span class="sxs-lookup"><span data-stu-id="110b7-122">String</span></span>|<span data-ttu-id="110b7-123">ID</span><span class="sxs-lookup"><span data-stu-id="110b7-123">The ID</span></span>|
|<span data-ttu-id="110b7-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="110b7-124">conflictCount</span></span>|<span data-ttu-id="110b7-125">Int32</span><span class="sxs-lookup"><span data-stu-id="110b7-125">Int32</span></span>|<span data-ttu-id="110b7-126">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="110b7-126">Number of users in conflict</span></span>|
|<span data-ttu-id="110b7-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="110b7-127">errorCount</span></span>|<span data-ttu-id="110b7-128">Int32</span><span class="sxs-lookup"><span data-stu-id="110b7-128">Int32</span></span>|<span data-ttu-id="110b7-129">错误用户数</span><span class="sxs-lookup"><span data-stu-id="110b7-129">Number of error users</span></span>|
|<span data-ttu-id="110b7-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="110b7-130">failedCount</span></span>|<span data-ttu-id="110b7-131">Int32</span><span class="sxs-lookup"><span data-stu-id="110b7-131">Int32</span></span>|<span data-ttu-id="110b7-132">失败的用户数</span><span class="sxs-lookup"><span data-stu-id="110b7-132">Number of failed users</span></span>|
|<span data-ttu-id="110b7-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="110b7-133">notApplicableCount</span></span>|<span data-ttu-id="110b7-134">Int32</span><span class="sxs-lookup"><span data-stu-id="110b7-134">Int32</span></span>|<span data-ttu-id="110b7-135">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="110b7-135">Number of not applicable users</span></span>|
|<span data-ttu-id="110b7-136">successCount</span><span class="sxs-lookup"><span data-stu-id="110b7-136">successCount</span></span>|<span data-ttu-id="110b7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="110b7-137">Int32</span></span>|<span data-ttu-id="110b7-138">成功的用户数</span><span class="sxs-lookup"><span data-stu-id="110b7-138">Number of succeeded users</span></span>|

## <a name="relationships"></a><span data-ttu-id="110b7-139">关系</span><span class="sxs-lookup"><span data-stu-id="110b7-139">Relationships</span></span>
<span data-ttu-id="110b7-140">无</span><span class="sxs-lookup"><span data-stu-id="110b7-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="110b7-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="110b7-141">JSON Representation</span></span>
<span data-ttu-id="110b7-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="110b7-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024
}
```








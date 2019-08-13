---
title: deviceManagementIntentUserStateSummary 资源类型
description: 表示意向的用户状态摘要的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c934dd2035b628b8424a75c0b95a2e642c67586c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364752"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a><span data-ttu-id="aa78b-103">deviceManagementIntentUserStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa78b-103">deviceManagementIntentUserStateSummary resource type</span></span>

> <span data-ttu-id="aa78b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aa78b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa78b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aa78b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa78b-106">表示意向的用户状态摘要的实体</span><span class="sxs-lookup"><span data-stu-id="aa78b-106">Entity that represents user state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="aa78b-107">方法</span><span class="sxs-lookup"><span data-stu-id="aa78b-107">Methods</span></span>
|<span data-ttu-id="aa78b-108">方法</span><span class="sxs-lookup"><span data-stu-id="aa78b-108">Method</span></span>|<span data-ttu-id="aa78b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="aa78b-109">Return Type</span></span>|<span data-ttu-id="aa78b-110">说明</span><span class="sxs-lookup"><span data-stu-id="aa78b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aa78b-111">获取 deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="aa78b-111">Get deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[<span data-ttu-id="aa78b-112">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="aa78b-112">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="aa78b-113">读取[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aa78b-113">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="aa78b-114">更新 deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="aa78b-114">Update deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[<span data-ttu-id="aa78b-115">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="aa78b-115">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="aa78b-116">更新[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aa78b-116">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa78b-117">属性</span><span class="sxs-lookup"><span data-stu-id="aa78b-117">Properties</span></span>
|<span data-ttu-id="aa78b-118">属性</span><span class="sxs-lookup"><span data-stu-id="aa78b-118">Property</span></span>|<span data-ttu-id="aa78b-119">类型</span><span class="sxs-lookup"><span data-stu-id="aa78b-119">Type</span></span>|<span data-ttu-id="aa78b-120">说明</span><span class="sxs-lookup"><span data-stu-id="aa78b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa78b-121">id</span><span class="sxs-lookup"><span data-stu-id="aa78b-121">id</span></span>|<span data-ttu-id="aa78b-122">String</span><span class="sxs-lookup"><span data-stu-id="aa78b-122">String</span></span>|<span data-ttu-id="aa78b-123">ID</span><span class="sxs-lookup"><span data-stu-id="aa78b-123">The ID</span></span>|
|<span data-ttu-id="aa78b-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="aa78b-124">conflictCount</span></span>|<span data-ttu-id="aa78b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="aa78b-125">Int32</span></span>|<span data-ttu-id="aa78b-126">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="aa78b-126">Number of users in conflict</span></span>|
|<span data-ttu-id="aa78b-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="aa78b-127">errorCount</span></span>|<span data-ttu-id="aa78b-128">Int32</span><span class="sxs-lookup"><span data-stu-id="aa78b-128">Int32</span></span>|<span data-ttu-id="aa78b-129">错误用户数</span><span class="sxs-lookup"><span data-stu-id="aa78b-129">Number of error users</span></span>|
|<span data-ttu-id="aa78b-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="aa78b-130">failedCount</span></span>|<span data-ttu-id="aa78b-131">Int32</span><span class="sxs-lookup"><span data-stu-id="aa78b-131">Int32</span></span>|<span data-ttu-id="aa78b-132">失败的用户数</span><span class="sxs-lookup"><span data-stu-id="aa78b-132">Number of failed users</span></span>|
|<span data-ttu-id="aa78b-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="aa78b-133">notApplicableCount</span></span>|<span data-ttu-id="aa78b-134">Int32</span><span class="sxs-lookup"><span data-stu-id="aa78b-134">Int32</span></span>|<span data-ttu-id="aa78b-135">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="aa78b-135">Number of not applicable users</span></span>|
|<span data-ttu-id="aa78b-136">successCount</span><span class="sxs-lookup"><span data-stu-id="aa78b-136">successCount</span></span>|<span data-ttu-id="aa78b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="aa78b-137">Int32</span></span>|<span data-ttu-id="aa78b-138">成功的用户数</span><span class="sxs-lookup"><span data-stu-id="aa78b-138">Number of succeeded users</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa78b-139">关系</span><span class="sxs-lookup"><span data-stu-id="aa78b-139">Relationships</span></span>
<span data-ttu-id="aa78b-140">无</span><span class="sxs-lookup"><span data-stu-id="aa78b-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa78b-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa78b-141">JSON Representation</span></span>
<span data-ttu-id="aa78b-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa78b-142">Here is a JSON representation of the resource.</span></span>
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




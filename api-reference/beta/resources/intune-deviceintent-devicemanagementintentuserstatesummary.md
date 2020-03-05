---
title: deviceManagementIntentUserStateSummary 资源类型
description: 表示意向的用户状态摘要的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc53020966717c2f9324e9fddef9b7f0173b0eb9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528823"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a><span data-ttu-id="cb663-103">deviceManagementIntentUserStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb663-103">deviceManagementIntentUserStateSummary resource type</span></span>

<span data-ttu-id="cb663-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cb663-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb663-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cb663-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb663-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cb663-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb663-107">表示意向的用户状态摘要的实体</span><span class="sxs-lookup"><span data-stu-id="cb663-107">Entity that represents user state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="cb663-108">方法</span><span class="sxs-lookup"><span data-stu-id="cb663-108">Methods</span></span>
|<span data-ttu-id="cb663-109">方法</span><span class="sxs-lookup"><span data-stu-id="cb663-109">Method</span></span>|<span data-ttu-id="cb663-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cb663-110">Return Type</span></span>|<span data-ttu-id="cb663-111">说明</span><span class="sxs-lookup"><span data-stu-id="cb663-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cb663-112">获取 deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="cb663-112">Get deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[<span data-ttu-id="cb663-113">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="cb663-113">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="cb663-114">读取[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cb663-114">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="cb663-115">更新 deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="cb663-115">Update deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[<span data-ttu-id="cb663-116">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="cb663-116">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="cb663-117">更新[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cb663-117">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cb663-118">属性</span><span class="sxs-lookup"><span data-stu-id="cb663-118">Properties</span></span>
|<span data-ttu-id="cb663-119">属性</span><span class="sxs-lookup"><span data-stu-id="cb663-119">Property</span></span>|<span data-ttu-id="cb663-120">类型</span><span class="sxs-lookup"><span data-stu-id="cb663-120">Type</span></span>|<span data-ttu-id="cb663-121">说明</span><span class="sxs-lookup"><span data-stu-id="cb663-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb663-122">id</span><span class="sxs-lookup"><span data-stu-id="cb663-122">id</span></span>|<span data-ttu-id="cb663-123">String</span><span class="sxs-lookup"><span data-stu-id="cb663-123">String</span></span>|<span data-ttu-id="cb663-124">ID</span><span class="sxs-lookup"><span data-stu-id="cb663-124">The ID</span></span>|
|<span data-ttu-id="cb663-125">conflictCount</span><span class="sxs-lookup"><span data-stu-id="cb663-125">conflictCount</span></span>|<span data-ttu-id="cb663-126">Int32</span><span class="sxs-lookup"><span data-stu-id="cb663-126">Int32</span></span>|<span data-ttu-id="cb663-127">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="cb663-127">Number of users in conflict</span></span>|
|<span data-ttu-id="cb663-128">errorCount</span><span class="sxs-lookup"><span data-stu-id="cb663-128">errorCount</span></span>|<span data-ttu-id="cb663-129">Int32</span><span class="sxs-lookup"><span data-stu-id="cb663-129">Int32</span></span>|<span data-ttu-id="cb663-130">错误用户数</span><span class="sxs-lookup"><span data-stu-id="cb663-130">Number of error users</span></span>|
|<span data-ttu-id="cb663-131">failedCount</span><span class="sxs-lookup"><span data-stu-id="cb663-131">failedCount</span></span>|<span data-ttu-id="cb663-132">Int32</span><span class="sxs-lookup"><span data-stu-id="cb663-132">Int32</span></span>|<span data-ttu-id="cb663-133">失败的用户数</span><span class="sxs-lookup"><span data-stu-id="cb663-133">Number of failed users</span></span>|
|<span data-ttu-id="cb663-134">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="cb663-134">notApplicableCount</span></span>|<span data-ttu-id="cb663-135">Int32</span><span class="sxs-lookup"><span data-stu-id="cb663-135">Int32</span></span>|<span data-ttu-id="cb663-136">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="cb663-136">Number of not applicable users</span></span>|
|<span data-ttu-id="cb663-137">successCount</span><span class="sxs-lookup"><span data-stu-id="cb663-137">successCount</span></span>|<span data-ttu-id="cb663-138">Int32</span><span class="sxs-lookup"><span data-stu-id="cb663-138">Int32</span></span>|<span data-ttu-id="cb663-139">成功的用户数</span><span class="sxs-lookup"><span data-stu-id="cb663-139">Number of succeeded users</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb663-140">关系</span><span class="sxs-lookup"><span data-stu-id="cb663-140">Relationships</span></span>
<span data-ttu-id="cb663-141">无</span><span class="sxs-lookup"><span data-stu-id="cb663-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb663-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb663-142">JSON Representation</span></span>
<span data-ttu-id="cb663-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb663-143">Here is a JSON representation of the resource.</span></span>
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




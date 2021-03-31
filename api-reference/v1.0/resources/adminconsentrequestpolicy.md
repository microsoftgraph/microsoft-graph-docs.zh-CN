---
title: adminConsentRequestPolicy 资源类型
description: 指定可在整个租户中创建和管理同意请求的策略。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7d7fadabdd8bc3581a2a32b70fad2b27c71c3b5c
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469543"
---
# <a name="adminconsentrequestpolicy-resource-type"></a><span data-ttu-id="3601b-103">adminConsentRequestPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="3601b-103">adminConsentRequestPolicy resource type</span></span>

<span data-ttu-id="3601b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3601b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3601b-105">指定创建和管理整个租户的同意请求的策略。</span><span class="sxs-lookup"><span data-stu-id="3601b-105">Specifies the policy by which consent requests are created and managed for the entire tenant.</span></span> <span data-ttu-id="3601b-106">每个租户只有一个 **adminConsentRequestPolicy。**</span><span class="sxs-lookup"><span data-stu-id="3601b-106">There is a single **adminConsentRequestPolicy** per tenant.</span></span>

<span data-ttu-id="3601b-107">**adminConsentRequestPolicy** 在创建同意请求时提供其他设置，以控制启动同意请求时的功能行为。</span><span class="sxs-lookup"><span data-stu-id="3601b-107">The **adminConsentRequestPolicy** provides additional settings when creating a consent request, to control the feature behavior when starting a consent request.</span></span>

## <a name="methods"></a><span data-ttu-id="3601b-108">方法</span><span class="sxs-lookup"><span data-stu-id="3601b-108">Methods</span></span>

|<span data-ttu-id="3601b-109">方法</span><span class="sxs-lookup"><span data-stu-id="3601b-109">Method</span></span>|<span data-ttu-id="3601b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="3601b-110">Return type</span></span>|<span data-ttu-id="3601b-111">说明</span><span class="sxs-lookup"><span data-stu-id="3601b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3601b-112">获取 adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="3601b-112">Get adminConsentRequestPolicy</span></span>](../api/adminconsentrequestpolicy-get.md)|[<span data-ttu-id="3601b-113">adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="3601b-113">adminConsentRequestPolicy</span></span>](../resources/adminconsentrequestpolicy.md)|<span data-ttu-id="3601b-114">读取 [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3601b-114">Read the properties and relationships of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>|
|[<span data-ttu-id="3601b-115">更新 adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="3601b-115">Update adminConsentRequestPolicy</span></span>](../api/adminconsentrequestpolicy-update.md)|[<span data-ttu-id="3601b-116">adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="3601b-116">adminConsentRequestPolicy</span></span>](../resources/adminconsentrequestpolicy.md)|<span data-ttu-id="3601b-117">更新 [adminConsentRequestPolicy 对象](../resources/adminconsentrequestpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="3601b-117">Update the properties of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3601b-118">属性</span><span class="sxs-lookup"><span data-stu-id="3601b-118">Properties</span></span>

|<span data-ttu-id="3601b-119">属性</span><span class="sxs-lookup"><span data-stu-id="3601b-119">Property</span></span>|<span data-ttu-id="3601b-120">类型</span><span class="sxs-lookup"><span data-stu-id="3601b-120">Type</span></span>|<span data-ttu-id="3601b-121">说明</span><span class="sxs-lookup"><span data-stu-id="3601b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3601b-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3601b-122">isEnabled</span></span>|<span data-ttu-id="3601b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="3601b-123">Boolean</span></span>|<span data-ttu-id="3601b-124">指定是启用还是禁用管理员同意请求功能。</span><span class="sxs-lookup"><span data-stu-id="3601b-124">Specifies whether the admin consent request feature is enabled or disabled.</span></span> <span data-ttu-id="3601b-125">必需。</span><span class="sxs-lookup"><span data-stu-id="3601b-125">Required.</span></span>|
|<span data-ttu-id="3601b-126">notifyReviewers</span><span class="sxs-lookup"><span data-stu-id="3601b-126">notifyReviewers</span></span>|<span data-ttu-id="3601b-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="3601b-127">Boolean</span></span>|<span data-ttu-id="3601b-128">指定审阅者是否将收到通知。</span><span class="sxs-lookup"><span data-stu-id="3601b-128">Specifies whether reviewers will receive notifications.</span></span> <span data-ttu-id="3601b-129">必需。</span><span class="sxs-lookup"><span data-stu-id="3601b-129">Required.</span></span>|
|<span data-ttu-id="3601b-130">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="3601b-130">remindersEnabled</span></span>|<span data-ttu-id="3601b-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="3601b-131">Boolean</span></span>|<span data-ttu-id="3601b-132">指定审阅者是否将收到提醒电子邮件。</span><span class="sxs-lookup"><span data-stu-id="3601b-132">Specifies whether reviewers will receive reminder emails.</span></span> <span data-ttu-id="3601b-133">必需。</span><span class="sxs-lookup"><span data-stu-id="3601b-133">Required.</span></span>|
|<span data-ttu-id="3601b-134">requestDurationInDays</span><span class="sxs-lookup"><span data-stu-id="3601b-134">requestDurationInDays</span></span>|<span data-ttu-id="3601b-135">Int32</span><span class="sxs-lookup"><span data-stu-id="3601b-135">Int32</span></span>|<span data-ttu-id="3601b-136">指定请求在未应用决策时自动过期之前处于活动状态的持续时间。</span><span class="sxs-lookup"><span data-stu-id="3601b-136">Specifies the duration the request is active before it automatically expires if no decision is applied.</span></span>|
|<span data-ttu-id="3601b-137">reviewers</span><span class="sxs-lookup"><span data-stu-id="3601b-137">reviewers</span></span>|<span data-ttu-id="3601b-138">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3601b-138">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="3601b-139">管理员同意的审阅者列表。</span><span class="sxs-lookup"><span data-stu-id="3601b-139">The list of reviewers for the admin consent.</span></span> <span data-ttu-id="3601b-140">必需。</span><span class="sxs-lookup"><span data-stu-id="3601b-140">Required.</span></span>|
|<span data-ttu-id="3601b-141">version</span><span class="sxs-lookup"><span data-stu-id="3601b-141">version</span></span>|<span data-ttu-id="3601b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="3601b-142">Int32</span></span>|<span data-ttu-id="3601b-143">指定此策略的版本。</span><span class="sxs-lookup"><span data-stu-id="3601b-143">Specifies the version of this policy.</span></span> <span data-ttu-id="3601b-144">更新策略时，将更新此版本。</span><span class="sxs-lookup"><span data-stu-id="3601b-144">When the policy is updated, this version is updated.</span></span> <span data-ttu-id="3601b-145">只读。</span><span class="sxs-lookup"><span data-stu-id="3601b-145">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3601b-146">关系</span><span class="sxs-lookup"><span data-stu-id="3601b-146">Relationships</span></span>

<span data-ttu-id="3601b-147">无。</span><span class="sxs-lookup"><span data-stu-id="3601b-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3601b-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3601b-148">JSON representation</span></span>

<span data-ttu-id="3601b-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3601b-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.adminConsentRequestPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsentRequestPolicy",
  "isEnabled": "Boolean",
  "version": "Integer",
  "notifyReviewers": "Boolean",
  "remindersEnabled": "Boolean",
  "requestDurationInDays": "Integer",
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ]
}
```


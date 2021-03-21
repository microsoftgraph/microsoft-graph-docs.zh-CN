---
title: adminConsentRequestPolicy 资源类型
description: 指定可在整个租户中创建和管理同意请求的策略。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dde04ac8c94f0f924df47f3b9490b09f18490c2c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965118"
---
# <a name="adminconsentrequestpolicy-resource-type"></a><span data-ttu-id="453d2-103">adminConsentRequestPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="453d2-103">adminConsentRequestPolicy resource type</span></span>

<span data-ttu-id="453d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="453d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="453d2-105">指定创建和管理整个租户的同意请求的策略。</span><span class="sxs-lookup"><span data-stu-id="453d2-105">Specifies the policy by which consent requests are created and managed for the entire tenant.</span></span> <span data-ttu-id="453d2-106">每个租户只有一个 **adminConsentRequestPolicy。**</span><span class="sxs-lookup"><span data-stu-id="453d2-106">There is a single **adminConsentRequestPolicy** per tenant.</span></span> 

<span data-ttu-id="453d2-107">**adminConsentRequestPolicy** 在创建同意请求时提供其他设置，以控制启动同意请求时的功能行为。</span><span class="sxs-lookup"><span data-stu-id="453d2-107">The **adminConsentRequestPolicy** provides additional settings when creating a consent request, to control the feature behavior when starting a consent request.</span></span>

## <a name="methods"></a><span data-ttu-id="453d2-108">Methods</span><span class="sxs-lookup"><span data-stu-id="453d2-108">Methods</span></span>
|<span data-ttu-id="453d2-109">方法</span><span class="sxs-lookup"><span data-stu-id="453d2-109">Method</span></span>|<span data-ttu-id="453d2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="453d2-110">Return type</span></span>|<span data-ttu-id="453d2-111">说明</span><span class="sxs-lookup"><span data-stu-id="453d2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="453d2-112">获取 adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="453d2-112">Get adminConsentRequestPolicy</span></span>](../api/adminconsentrequestpolicy-get.md)|[<span data-ttu-id="453d2-113">adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="453d2-113">adminConsentRequestPolicy</span></span>](../resources/adminconsentrequestpolicy.md)|<span data-ttu-id="453d2-114">读取 [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="453d2-114">Read the properties and relationships of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>|
|[<span data-ttu-id="453d2-115">更新 adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="453d2-115">Update adminConsentRequestPolicy</span></span>](../api/adminconsentrequestpolicy-update.md)|[<span data-ttu-id="453d2-116">adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="453d2-116">adminConsentRequestPolicy</span></span>](../resources/adminconsentrequestpolicy.md)|<span data-ttu-id="453d2-117">更新 [adminConsentRequestPolicy 对象](../resources/adminconsentrequestpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="453d2-117">Update the properties of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="453d2-118">属性</span><span class="sxs-lookup"><span data-stu-id="453d2-118">Properties</span></span>
|<span data-ttu-id="453d2-119">属性</span><span class="sxs-lookup"><span data-stu-id="453d2-119">Property</span></span>|<span data-ttu-id="453d2-120">类型</span><span class="sxs-lookup"><span data-stu-id="453d2-120">Type</span></span>|<span data-ttu-id="453d2-121">说明</span><span class="sxs-lookup"><span data-stu-id="453d2-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="453d2-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="453d2-122">isEnabled</span></span>|<span data-ttu-id="453d2-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="453d2-123">Boolean</span></span>|<span data-ttu-id="453d2-124">指定是启用还是禁用管理员同意请求功能。</span><span class="sxs-lookup"><span data-stu-id="453d2-124">Specifies whether the admin consent request feature is enabled or disabled.</span></span> <span data-ttu-id="453d2-125">必填。</span><span class="sxs-lookup"><span data-stu-id="453d2-125">Required.</span></span>|
|<span data-ttu-id="453d2-126">notifyReviewers</span><span class="sxs-lookup"><span data-stu-id="453d2-126">notifyReviewers</span></span>|<span data-ttu-id="453d2-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="453d2-127">Boolean</span></span>|<span data-ttu-id="453d2-128">指定审阅者是否将收到通知。</span><span class="sxs-lookup"><span data-stu-id="453d2-128">Specifies whether reviewers will receive notifications.</span></span> <span data-ttu-id="453d2-129">必填。</span><span class="sxs-lookup"><span data-stu-id="453d2-129">Required.</span></span>|
|<span data-ttu-id="453d2-130">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="453d2-130">remindersEnabled</span></span>|<span data-ttu-id="453d2-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="453d2-131">Boolean</span></span>|<span data-ttu-id="453d2-132">指定审阅者是否将收到提醒电子邮件。</span><span class="sxs-lookup"><span data-stu-id="453d2-132">Specifies whether reviewers will receive reminder emails.</span></span> <span data-ttu-id="453d2-133">必填。</span><span class="sxs-lookup"><span data-stu-id="453d2-133">Required.</span></span>|
|<span data-ttu-id="453d2-134">requestDurationInDays</span><span class="sxs-lookup"><span data-stu-id="453d2-134">requestDurationInDays</span></span>|<span data-ttu-id="453d2-135">Int32</span><span class="sxs-lookup"><span data-stu-id="453d2-135">Int32</span></span>|<span data-ttu-id="453d2-136">指定请求在未应用决策时自动过期之前处于活动状态的持续时间。</span><span class="sxs-lookup"><span data-stu-id="453d2-136">Specifies the duration the request is active before it automatically expires if no decision is applied.</span></span>|
|<span data-ttu-id="453d2-137">reviewers</span><span class="sxs-lookup"><span data-stu-id="453d2-137">reviewers</span></span>|<span data-ttu-id="453d2-138">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="453d2-138">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="453d2-139">必填。</span><span class="sxs-lookup"><span data-stu-id="453d2-139">Required.</span></span>|
|<span data-ttu-id="453d2-140">version</span><span class="sxs-lookup"><span data-stu-id="453d2-140">version</span></span>|<span data-ttu-id="453d2-141">Int32</span><span class="sxs-lookup"><span data-stu-id="453d2-141">Int32</span></span>|<span data-ttu-id="453d2-142">指定此策略的版本。</span><span class="sxs-lookup"><span data-stu-id="453d2-142">Specifies the version of this policy.</span></span> <span data-ttu-id="453d2-143">更新策略时，将更新此版本。</span><span class="sxs-lookup"><span data-stu-id="453d2-143">When the policy is updated, this version is updated.</span></span> <span data-ttu-id="453d2-144">只读。</span><span class="sxs-lookup"><span data-stu-id="453d2-144">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="453d2-145">关系</span><span class="sxs-lookup"><span data-stu-id="453d2-145">Relationships</span></span>
<span data-ttu-id="453d2-146">无。</span><span class="sxs-lookup"><span data-stu-id="453d2-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="453d2-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="453d2-147">JSON representation</span></span>
<span data-ttu-id="453d2-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="453d2-148">The following is a JSON representation of the resource.</span></span>
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

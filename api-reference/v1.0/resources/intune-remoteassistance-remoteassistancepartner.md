---
title: remoteAssistancePartner 资源类型
description: remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0557eb45fb770c257f1734bf967f78e9e00cac81
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253251"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="58c83-103">remoteAssistancePartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="58c83-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="58c83-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58c83-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58c83-105">remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="58c83-105">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="58c83-106">方法</span><span class="sxs-lookup"><span data-stu-id="58c83-106">Methods</span></span>
|<span data-ttu-id="58c83-107">方法</span><span class="sxs-lookup"><span data-stu-id="58c83-107">Method</span></span>|<span data-ttu-id="58c83-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="58c83-108">Return Type</span></span>|<span data-ttu-id="58c83-109">说明</span><span class="sxs-lookup"><span data-stu-id="58c83-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="58c83-110">列出 remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="58c83-110">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="58c83-111">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="58c83-111">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="58c83-112">列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="58c83-112">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="58c83-113">获取 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="58c83-113">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="58c83-114">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="58c83-114">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="58c83-115">读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="58c83-115">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="58c83-116">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="58c83-116">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="58c83-117">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="58c83-117">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="58c83-118">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58c83-118">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="58c83-119">删除 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="58c83-119">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="58c83-120">无</span><span class="sxs-lookup"><span data-stu-id="58c83-120">None</span></span>|<span data-ttu-id="58c83-121">删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。</span><span class="sxs-lookup"><span data-stu-id="58c83-121">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="58c83-122">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="58c83-122">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="58c83-123">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="58c83-123">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="58c83-124">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="58c83-124">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="58c83-125">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="58c83-125">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="58c83-126">无</span><span class="sxs-lookup"><span data-stu-id="58c83-126">None</span></span>|<span data-ttu-id="58c83-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="58c83-127">Not yet documented</span></span>|
|[<span data-ttu-id="58c83-128">断开连接操作</span><span class="sxs-lookup"><span data-stu-id="58c83-128">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="58c83-129">无</span><span class="sxs-lookup"><span data-stu-id="58c83-129">None</span></span>|<span data-ttu-id="58c83-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="58c83-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="58c83-131">属性</span><span class="sxs-lookup"><span data-stu-id="58c83-131">Properties</span></span>
|<span data-ttu-id="58c83-132">属性</span><span class="sxs-lookup"><span data-stu-id="58c83-132">Property</span></span>|<span data-ttu-id="58c83-133">类型</span><span class="sxs-lookup"><span data-stu-id="58c83-133">Type</span></span>|<span data-ttu-id="58c83-134">说明</span><span class="sxs-lookup"><span data-stu-id="58c83-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58c83-135">id</span><span class="sxs-lookup"><span data-stu-id="58c83-135">id</span></span>|<span data-ttu-id="58c83-136">字符串</span><span class="sxs-lookup"><span data-stu-id="58c83-136">String</span></span>|<span data-ttu-id="58c83-137">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="58c83-137">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="58c83-138">displayName</span><span class="sxs-lookup"><span data-stu-id="58c83-138">displayName</span></span>|<span data-ttu-id="58c83-139">String</span><span class="sxs-lookup"><span data-stu-id="58c83-139">String</span></span>|<span data-ttu-id="58c83-140">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="58c83-140">Display name of the partner.</span></span>|
|<span data-ttu-id="58c83-141">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="58c83-141">onboardingUrl</span></span>|<span data-ttu-id="58c83-142">String</span><span class="sxs-lookup"><span data-stu-id="58c83-142">String</span></span>|<span data-ttu-id="58c83-143">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="58c83-143">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="58c83-144">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="58c83-144">onboardingStatus</span></span>|[<span data-ttu-id="58c83-145">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="58c83-145">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="58c83-146">待定.</span><span class="sxs-lookup"><span data-stu-id="58c83-146">TBD.</span></span> <span data-ttu-id="58c83-147">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="58c83-147">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="58c83-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="58c83-148">lastConnectionDateTime</span></span>|<span data-ttu-id="58c83-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58c83-149">DateTimeOffset</span></span>|<span data-ttu-id="58c83-150">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="58c83-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58c83-151">关系</span><span class="sxs-lookup"><span data-stu-id="58c83-151">Relationships</span></span>
<span data-ttu-id="58c83-152">无</span><span class="sxs-lookup"><span data-stu-id="58c83-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58c83-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58c83-153">JSON Representation</span></span>
<span data-ttu-id="58c83-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58c83-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```




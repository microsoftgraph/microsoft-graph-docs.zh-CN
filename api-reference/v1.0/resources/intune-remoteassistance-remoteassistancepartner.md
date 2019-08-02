---
title: remoteAssistancePartner 资源类型
description: remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7bd14d3978e629c75ee9c232a07f88446ca545d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037049"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="fb029-103">remoteAssistancePartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb029-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="fb029-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb029-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb029-105">remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="fb029-105">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="fb029-106">方法</span><span class="sxs-lookup"><span data-stu-id="fb029-106">Methods</span></span>
|<span data-ttu-id="fb029-107">方法</span><span class="sxs-lookup"><span data-stu-id="fb029-107">Method</span></span>|<span data-ttu-id="fb029-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="fb029-108">Return Type</span></span>|<span data-ttu-id="fb029-109">说明</span><span class="sxs-lookup"><span data-stu-id="fb029-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fb029-110">列出 remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="fb029-110">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="fb029-111">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fb029-111">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="fb029-112">列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fb029-112">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="fb029-113">获取 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fb029-113">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="fb029-114">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fb029-114">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="fb029-115">读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fb029-115">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="fb029-116">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fb029-116">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="fb029-117">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fb029-117">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="fb029-118">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb029-118">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="fb029-119">删除 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fb029-119">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="fb029-120">无</span><span class="sxs-lookup"><span data-stu-id="fb029-120">None</span></span>|<span data-ttu-id="fb029-121">删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。</span><span class="sxs-lookup"><span data-stu-id="fb029-121">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="fb029-122">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fb029-122">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="fb029-123">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fb029-123">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="fb029-124">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fb029-124">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="fb029-125">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="fb029-125">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="fb029-126">无</span><span class="sxs-lookup"><span data-stu-id="fb029-126">None</span></span>|<span data-ttu-id="fb029-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fb029-127">Not yet documented</span></span>|
|[<span data-ttu-id="fb029-128">断开连接操作</span><span class="sxs-lookup"><span data-stu-id="fb029-128">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="fb029-129">无</span><span class="sxs-lookup"><span data-stu-id="fb029-129">None</span></span>|<span data-ttu-id="fb029-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fb029-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fb029-131">属性</span><span class="sxs-lookup"><span data-stu-id="fb029-131">Properties</span></span>
|<span data-ttu-id="fb029-132">属性</span><span class="sxs-lookup"><span data-stu-id="fb029-132">Property</span></span>|<span data-ttu-id="fb029-133">类型</span><span class="sxs-lookup"><span data-stu-id="fb029-133">Type</span></span>|<span data-ttu-id="fb029-134">说明</span><span class="sxs-lookup"><span data-stu-id="fb029-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb029-135">id</span><span class="sxs-lookup"><span data-stu-id="fb029-135">id</span></span>|<span data-ttu-id="fb029-136">String</span><span class="sxs-lookup"><span data-stu-id="fb029-136">String</span></span>|<span data-ttu-id="fb029-137">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fb029-137">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="fb029-138">displayName</span><span class="sxs-lookup"><span data-stu-id="fb029-138">displayName</span></span>|<span data-ttu-id="fb029-139">字符串</span><span class="sxs-lookup"><span data-stu-id="fb029-139">String</span></span>|<span data-ttu-id="fb029-140">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fb029-140">Display name of the partner.</span></span>|
|<span data-ttu-id="fb029-141">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="fb029-141">onboardingUrl</span></span>|<span data-ttu-id="fb029-142">String</span><span class="sxs-lookup"><span data-stu-id="fb029-142">String</span></span>|<span data-ttu-id="fb029-143">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="fb029-143">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="fb029-144">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="fb029-144">onboardingStatus</span></span>|[<span data-ttu-id="fb029-145">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="fb029-145">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="fb029-146">待定.</span><span class="sxs-lookup"><span data-stu-id="fb029-146">TBD.</span></span> <span data-ttu-id="fb029-147">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="fb029-147">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="fb029-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="fb029-148">lastConnectionDateTime</span></span>|<span data-ttu-id="fb029-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb029-149">DateTimeOffset</span></span>|<span data-ttu-id="fb029-150">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="fb029-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb029-151">关系</span><span class="sxs-lookup"><span data-stu-id="fb029-151">Relationships</span></span>
<span data-ttu-id="fb029-152">无</span><span class="sxs-lookup"><span data-stu-id="fb029-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb029-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb029-153">JSON Representation</span></span>
<span data-ttu-id="fb029-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb029-154">Here is a JSON representation of the resource.</span></span>
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




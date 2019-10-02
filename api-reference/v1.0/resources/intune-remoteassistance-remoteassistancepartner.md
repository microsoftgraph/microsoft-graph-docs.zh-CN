---
title: remoteAssistancePartner 资源类型
description: remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc989eb09b84102130dad7cce2b55ae785452f00
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355867"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="1284d-103">remoteAssistancePartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="1284d-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="1284d-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1284d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1284d-105">remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="1284d-105">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="1284d-106">方法</span><span class="sxs-lookup"><span data-stu-id="1284d-106">Methods</span></span>
|<span data-ttu-id="1284d-107">方法</span><span class="sxs-lookup"><span data-stu-id="1284d-107">Method</span></span>|<span data-ttu-id="1284d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1284d-108">Return Type</span></span>|<span data-ttu-id="1284d-109">说明</span><span class="sxs-lookup"><span data-stu-id="1284d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1284d-110">列出 remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="1284d-110">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="1284d-111">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1284d-111">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="1284d-112">列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1284d-112">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="1284d-113">获取 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1284d-113">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="1284d-114">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1284d-114">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="1284d-115">读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1284d-115">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="1284d-116">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1284d-116">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="1284d-117">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1284d-117">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="1284d-118">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1284d-118">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="1284d-119">删除 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1284d-119">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="1284d-120">无</span><span class="sxs-lookup"><span data-stu-id="1284d-120">None</span></span>|<span data-ttu-id="1284d-121">删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。</span><span class="sxs-lookup"><span data-stu-id="1284d-121">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="1284d-122">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1284d-122">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="1284d-123">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1284d-123">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="1284d-124">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1284d-124">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="1284d-125">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="1284d-125">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="1284d-126">无</span><span class="sxs-lookup"><span data-stu-id="1284d-126">None</span></span>|<span data-ttu-id="1284d-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1284d-127">Not yet documented</span></span>|
|[<span data-ttu-id="1284d-128">断开连接操作</span><span class="sxs-lookup"><span data-stu-id="1284d-128">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="1284d-129">无</span><span class="sxs-lookup"><span data-stu-id="1284d-129">None</span></span>|<span data-ttu-id="1284d-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1284d-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1284d-131">属性</span><span class="sxs-lookup"><span data-stu-id="1284d-131">Properties</span></span>
|<span data-ttu-id="1284d-132">属性</span><span class="sxs-lookup"><span data-stu-id="1284d-132">Property</span></span>|<span data-ttu-id="1284d-133">类型</span><span class="sxs-lookup"><span data-stu-id="1284d-133">Type</span></span>|<span data-ttu-id="1284d-134">说明</span><span class="sxs-lookup"><span data-stu-id="1284d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1284d-135">id</span><span class="sxs-lookup"><span data-stu-id="1284d-135">id</span></span>|<span data-ttu-id="1284d-136">String</span><span class="sxs-lookup"><span data-stu-id="1284d-136">String</span></span>|<span data-ttu-id="1284d-137">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1284d-137">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="1284d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="1284d-138">displayName</span></span>|<span data-ttu-id="1284d-139">字符串</span><span class="sxs-lookup"><span data-stu-id="1284d-139">String</span></span>|<span data-ttu-id="1284d-140">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1284d-140">Display name of the partner.</span></span>|
|<span data-ttu-id="1284d-141">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="1284d-141">onboardingUrl</span></span>|<span data-ttu-id="1284d-142">String</span><span class="sxs-lookup"><span data-stu-id="1284d-142">String</span></span>|<span data-ttu-id="1284d-143">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="1284d-143">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="1284d-144">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="1284d-144">onboardingStatus</span></span>|[<span data-ttu-id="1284d-145">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="1284d-145">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="1284d-146">待定.</span><span class="sxs-lookup"><span data-stu-id="1284d-146">TBD.</span></span> <span data-ttu-id="1284d-147">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="1284d-147">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="1284d-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="1284d-148">lastConnectionDateTime</span></span>|<span data-ttu-id="1284d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1284d-149">DateTimeOffset</span></span>|<span data-ttu-id="1284d-150">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="1284d-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1284d-151">关系</span><span class="sxs-lookup"><span data-stu-id="1284d-151">Relationships</span></span>
<span data-ttu-id="1284d-152">无</span><span class="sxs-lookup"><span data-stu-id="1284d-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1284d-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1284d-153">JSON Representation</span></span>
<span data-ttu-id="1284d-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1284d-154">Here is a JSON representation of the resource.</span></span>
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





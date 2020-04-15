---
title: remoteAssistancePartner 资源类型
description: remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9eca68f2a2feb2906f1d2b55b3f857d515a22c50
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441555"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="54e83-103">remoteAssistancePartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="54e83-103">remoteAssistancePartner resource type</span></span>

<span data-ttu-id="54e83-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54e83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54e83-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54e83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54e83-106">remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="54e83-106">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="54e83-107">方法</span><span class="sxs-lookup"><span data-stu-id="54e83-107">Methods</span></span>
|<span data-ttu-id="54e83-108">方法</span><span class="sxs-lookup"><span data-stu-id="54e83-108">Method</span></span>|<span data-ttu-id="54e83-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="54e83-109">Return Type</span></span>|<span data-ttu-id="54e83-110">说明</span><span class="sxs-lookup"><span data-stu-id="54e83-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="54e83-111">列出 remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="54e83-111">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="54e83-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="54e83-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="54e83-113">列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="54e83-113">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="54e83-114">获取 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="54e83-114">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="54e83-115">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="54e83-115">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="54e83-116">读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="54e83-116">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="54e83-117">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="54e83-117">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="54e83-118">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="54e83-118">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="54e83-119">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="54e83-119">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="54e83-120">删除 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="54e83-120">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="54e83-121">无</span><span class="sxs-lookup"><span data-stu-id="54e83-121">None</span></span>|<span data-ttu-id="54e83-122">删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。</span><span class="sxs-lookup"><span data-stu-id="54e83-122">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="54e83-123">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="54e83-123">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="54e83-124">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="54e83-124">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="54e83-125">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="54e83-125">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="54e83-126">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="54e83-126">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="54e83-127">无</span><span class="sxs-lookup"><span data-stu-id="54e83-127">None</span></span>|<span data-ttu-id="54e83-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="54e83-128">Not yet documented</span></span>|
|[<span data-ttu-id="54e83-129">断开连接操作</span><span class="sxs-lookup"><span data-stu-id="54e83-129">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="54e83-130">无</span><span class="sxs-lookup"><span data-stu-id="54e83-130">None</span></span>|<span data-ttu-id="54e83-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="54e83-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="54e83-132">属性</span><span class="sxs-lookup"><span data-stu-id="54e83-132">Properties</span></span>
|<span data-ttu-id="54e83-133">属性</span><span class="sxs-lookup"><span data-stu-id="54e83-133">Property</span></span>|<span data-ttu-id="54e83-134">类型</span><span class="sxs-lookup"><span data-stu-id="54e83-134">Type</span></span>|<span data-ttu-id="54e83-135">说明</span><span class="sxs-lookup"><span data-stu-id="54e83-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54e83-136">id</span><span class="sxs-lookup"><span data-stu-id="54e83-136">id</span></span>|<span data-ttu-id="54e83-137">String</span><span class="sxs-lookup"><span data-stu-id="54e83-137">String</span></span>|<span data-ttu-id="54e83-138">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="54e83-138">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="54e83-139">displayName</span><span class="sxs-lookup"><span data-stu-id="54e83-139">displayName</span></span>|<span data-ttu-id="54e83-140">字符串</span><span class="sxs-lookup"><span data-stu-id="54e83-140">String</span></span>|<span data-ttu-id="54e83-141">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="54e83-141">Display name of the partner.</span></span>|
|<span data-ttu-id="54e83-142">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="54e83-142">onboardingUrl</span></span>|<span data-ttu-id="54e83-143">String</span><span class="sxs-lookup"><span data-stu-id="54e83-143">String</span></span>|<span data-ttu-id="54e83-144">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="54e83-144">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="54e83-145">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="54e83-145">onboardingStatus</span></span>|[<span data-ttu-id="54e83-146">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="54e83-146">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="54e83-147">待定.</span><span class="sxs-lookup"><span data-stu-id="54e83-147">TBD.</span></span> <span data-ttu-id="54e83-148">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="54e83-148">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="54e83-149">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="54e83-149">lastConnectionDateTime</span></span>|<span data-ttu-id="54e83-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54e83-150">DateTimeOffset</span></span>|<span data-ttu-id="54e83-151">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="54e83-151">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54e83-152">关系</span><span class="sxs-lookup"><span data-stu-id="54e83-152">Relationships</span></span>
<span data-ttu-id="54e83-153">无</span><span class="sxs-lookup"><span data-stu-id="54e83-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54e83-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54e83-154">JSON Representation</span></span>
<span data-ttu-id="54e83-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54e83-155">Here is a JSON representation of the resource.</span></span>
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








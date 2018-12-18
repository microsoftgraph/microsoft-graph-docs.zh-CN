---
title: remoteAssistancePartner 资源类型
description: remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。
author: tfitzmac
ms.openlocfilehash: cb4dee80995f00d82cb1ba95f40dd31b1b82f48c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309188"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="9afb7-103">remoteAssistancePartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="9afb7-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="9afb7-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9afb7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9afb7-105">remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="9afb7-105">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>
## <a name="methods"></a><span data-ttu-id="9afb7-106">方法</span><span class="sxs-lookup"><span data-stu-id="9afb7-106">Methods</span></span>
|<span data-ttu-id="9afb7-107">方法</span><span class="sxs-lookup"><span data-stu-id="9afb7-107">Method</span></span>|<span data-ttu-id="9afb7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9afb7-108">Return Type</span></span>|<span data-ttu-id="9afb7-109">说明</span><span class="sxs-lookup"><span data-stu-id="9afb7-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9afb7-110">列出 remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="9afb7-110">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="9afb7-111">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9afb7-111">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="9afb7-112">列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9afb7-112">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="9afb7-113">获取 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="9afb7-113">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="9afb7-114">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="9afb7-114">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="9afb7-115">读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9afb7-115">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="9afb7-116">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="9afb7-116">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="9afb7-117">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="9afb7-117">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="9afb7-118">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9afb7-118">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="9afb7-119">删除 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="9afb7-119">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="9afb7-120">无</span><span class="sxs-lookup"><span data-stu-id="9afb7-120">None</span></span>|<span data-ttu-id="9afb7-121">删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。</span><span class="sxs-lookup"><span data-stu-id="9afb7-121">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="9afb7-122">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="9afb7-122">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="9afb7-123">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="9afb7-123">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="9afb7-124">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9afb7-124">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="9afb7-125">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="9afb7-125">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="9afb7-126">无</span><span class="sxs-lookup"><span data-stu-id="9afb7-126">None</span></span>|<span data-ttu-id="9afb7-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9afb7-127">Not yet documented</span></span>|
|[<span data-ttu-id="9afb7-128">断开连接操作</span><span class="sxs-lookup"><span data-stu-id="9afb7-128">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="9afb7-129">无</span><span class="sxs-lookup"><span data-stu-id="9afb7-129">None</span></span>|<span data-ttu-id="9afb7-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9afb7-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9afb7-131">属性</span><span class="sxs-lookup"><span data-stu-id="9afb7-131">Properties</span></span>
|<span data-ttu-id="9afb7-132">属性</span><span class="sxs-lookup"><span data-stu-id="9afb7-132">Property</span></span>|<span data-ttu-id="9afb7-133">类型</span><span class="sxs-lookup"><span data-stu-id="9afb7-133">Type</span></span>|<span data-ttu-id="9afb7-134">说明</span><span class="sxs-lookup"><span data-stu-id="9afb7-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9afb7-135">id</span><span class="sxs-lookup"><span data-stu-id="9afb7-135">id</span></span>|<span data-ttu-id="9afb7-136">String</span><span class="sxs-lookup"><span data-stu-id="9afb7-136">String</span></span>|<span data-ttu-id="9afb7-137">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9afb7-137">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="9afb7-138">displayName</span><span class="sxs-lookup"><span data-stu-id="9afb7-138">displayName</span></span>|<span data-ttu-id="9afb7-139">String</span><span class="sxs-lookup"><span data-stu-id="9afb7-139">String</span></span>|<span data-ttu-id="9afb7-140">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9afb7-140">Display name of the partner.</span></span>|
|<span data-ttu-id="9afb7-141">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="9afb7-141">onboardingUrl</span></span>|<span data-ttu-id="9afb7-142">String</span><span class="sxs-lookup"><span data-stu-id="9afb7-142">String</span></span>|<span data-ttu-id="9afb7-143">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="9afb7-143">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="9afb7-144">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="9afb7-144">onboardingStatus</span></span>|[<span data-ttu-id="9afb7-145">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="9afb7-145">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="9afb7-146">TBD。</span><span class="sxs-lookup"><span data-stu-id="9afb7-146">TBD.</span></span> <span data-ttu-id="9afb7-147">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="9afb7-147">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="9afb7-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="9afb7-148">lastConnectionDateTime</span></span>|<span data-ttu-id="9afb7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9afb7-149">DateTimeOffset</span></span>|<span data-ttu-id="9afb7-150">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="9afb7-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9afb7-151">关系</span><span class="sxs-lookup"><span data-stu-id="9afb7-151">Relationships</span></span>
<span data-ttu-id="9afb7-152">无</span><span class="sxs-lookup"><span data-stu-id="9afb7-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9afb7-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9afb7-153">JSON Representation</span></span>
<span data-ttu-id="9afb7-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9afb7-154">Here is a JSON representation of the resource.</span></span>
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




---
title: remoteAssistancePartner 资源类型
description: remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。
author: tfitzmac
ms.openlocfilehash: d3027ced433112b275d74d8c910553d5001d93ef
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344588"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="87908-103">remoteAssistancePartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="87908-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="87908-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="87908-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87908-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="87908-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87908-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="87908-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87908-107">remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="87908-107">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>
## <a name="methods"></a><span data-ttu-id="87908-108">方法</span><span class="sxs-lookup"><span data-stu-id="87908-108">Methods</span></span>
|<span data-ttu-id="87908-109">方法</span><span class="sxs-lookup"><span data-stu-id="87908-109">Method</span></span>|<span data-ttu-id="87908-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="87908-110">Return Type</span></span>|<span data-ttu-id="87908-111">说明</span><span class="sxs-lookup"><span data-stu-id="87908-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="87908-112">列出 remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="87908-112">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="87908-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="87908-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="87908-114">列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="87908-114">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="87908-115">获取 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="87908-115">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="87908-116">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="87908-116">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="87908-117">读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="87908-117">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="87908-118">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="87908-118">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="87908-119">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="87908-119">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="87908-120">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="87908-120">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="87908-121">删除 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="87908-121">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="87908-122">无</span><span class="sxs-lookup"><span data-stu-id="87908-122">None</span></span>|<span data-ttu-id="87908-123">删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。</span><span class="sxs-lookup"><span data-stu-id="87908-123">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="87908-124">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="87908-124">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="87908-125">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="87908-125">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="87908-126">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="87908-126">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="87908-127">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="87908-127">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="87908-128">无</span><span class="sxs-lookup"><span data-stu-id="87908-128">None</span></span>|<span data-ttu-id="87908-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="87908-129">Not yet documented</span></span>|
|[<span data-ttu-id="87908-130">断开连接操作</span><span class="sxs-lookup"><span data-stu-id="87908-130">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="87908-131">无</span><span class="sxs-lookup"><span data-stu-id="87908-131">None</span></span>|<span data-ttu-id="87908-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="87908-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="87908-133">属性</span><span class="sxs-lookup"><span data-stu-id="87908-133">Properties</span></span>
|<span data-ttu-id="87908-134">属性</span><span class="sxs-lookup"><span data-stu-id="87908-134">Property</span></span>|<span data-ttu-id="87908-135">类型</span><span class="sxs-lookup"><span data-stu-id="87908-135">Type</span></span>|<span data-ttu-id="87908-136">说明</span><span class="sxs-lookup"><span data-stu-id="87908-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87908-137">id</span><span class="sxs-lookup"><span data-stu-id="87908-137">id</span></span>|<span data-ttu-id="87908-138">String</span><span class="sxs-lookup"><span data-stu-id="87908-138">String</span></span>|<span data-ttu-id="87908-139">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="87908-139">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="87908-140">displayName</span><span class="sxs-lookup"><span data-stu-id="87908-140">displayName</span></span>|<span data-ttu-id="87908-141">String</span><span class="sxs-lookup"><span data-stu-id="87908-141">String</span></span>|<span data-ttu-id="87908-142">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="87908-142">Display name of the partner.</span></span>|
|<span data-ttu-id="87908-143">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="87908-143">onboardingUrl</span></span>|<span data-ttu-id="87908-144">String</span><span class="sxs-lookup"><span data-stu-id="87908-144">String</span></span>|<span data-ttu-id="87908-145">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="87908-145">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="87908-146">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="87908-146">onboardingStatus</span></span>|[<span data-ttu-id="87908-147">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="87908-147">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="87908-148">TBD。</span><span class="sxs-lookup"><span data-stu-id="87908-148">TBD.</span></span> <span data-ttu-id="87908-149">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="87908-149">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="87908-150">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="87908-150">lastConnectionDateTime</span></span>|<span data-ttu-id="87908-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87908-151">DateTimeOffset</span></span>|<span data-ttu-id="87908-152">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="87908-152">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87908-153">关系</span><span class="sxs-lookup"><span data-stu-id="87908-153">Relationships</span></span>
<span data-ttu-id="87908-154">无</span><span class="sxs-lookup"><span data-stu-id="87908-154">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="87908-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87908-155">JSON Representation</span></span>
<span data-ttu-id="87908-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87908-156">Here is a JSON representation of the resource.</span></span>
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






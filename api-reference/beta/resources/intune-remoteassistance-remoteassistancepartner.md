---
title: remoteAssistancePartner 资源类型
description: remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。
ms.openlocfilehash: 64ba3aacdeeb421f02b5affd94ecdbcb18ffd446
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045149"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="be43f-103">remoteAssistancePartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="be43f-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="be43f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="be43f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be43f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="be43f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be43f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="be43f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be43f-107">remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="be43f-107">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>
## <a name="methods"></a><span data-ttu-id="be43f-108">方法</span><span class="sxs-lookup"><span data-stu-id="be43f-108">Methods</span></span>
|<span data-ttu-id="be43f-109">方法</span><span class="sxs-lookup"><span data-stu-id="be43f-109">Method</span></span>|<span data-ttu-id="be43f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="be43f-110">Return Type</span></span>|<span data-ttu-id="be43f-111">说明</span><span class="sxs-lookup"><span data-stu-id="be43f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be43f-112">列出 remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="be43f-112">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="be43f-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be43f-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="be43f-114">列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be43f-114">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="be43f-115">获取 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="be43f-115">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="be43f-116">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="be43f-116">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="be43f-117">读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be43f-117">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="be43f-118">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="be43f-118">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="be43f-119">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="be43f-119">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="be43f-120">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be43f-120">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="be43f-121">删除 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="be43f-121">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="be43f-122">无</span><span class="sxs-lookup"><span data-stu-id="be43f-122">None</span></span>|<span data-ttu-id="be43f-123">删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。</span><span class="sxs-lookup"><span data-stu-id="be43f-123">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="be43f-124">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="be43f-124">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="be43f-125">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="be43f-125">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="be43f-126">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="be43f-126">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="be43f-127">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="be43f-127">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="be43f-128">无</span><span class="sxs-lookup"><span data-stu-id="be43f-128">None</span></span>|<span data-ttu-id="be43f-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="be43f-129">Not yet documented</span></span>|
|[<span data-ttu-id="be43f-130">断开连接操作</span><span class="sxs-lookup"><span data-stu-id="be43f-130">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="be43f-131">无</span><span class="sxs-lookup"><span data-stu-id="be43f-131">None</span></span>|<span data-ttu-id="be43f-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="be43f-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="be43f-133">属性</span><span class="sxs-lookup"><span data-stu-id="be43f-133">Properties</span></span>
|<span data-ttu-id="be43f-134">属性</span><span class="sxs-lookup"><span data-stu-id="be43f-134">Property</span></span>|<span data-ttu-id="be43f-135">类型</span><span class="sxs-lookup"><span data-stu-id="be43f-135">Type</span></span>|<span data-ttu-id="be43f-136">说明</span><span class="sxs-lookup"><span data-stu-id="be43f-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be43f-137">id</span><span class="sxs-lookup"><span data-stu-id="be43f-137">id</span></span>|<span data-ttu-id="be43f-138">String</span><span class="sxs-lookup"><span data-stu-id="be43f-138">String</span></span>|<span data-ttu-id="be43f-139">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="be43f-139">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="be43f-140">displayName</span><span class="sxs-lookup"><span data-stu-id="be43f-140">displayName</span></span>|<span data-ttu-id="be43f-141">String</span><span class="sxs-lookup"><span data-stu-id="be43f-141">String</span></span>|<span data-ttu-id="be43f-142">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="be43f-142">Display name of the partner.</span></span>|
|<span data-ttu-id="be43f-143">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="be43f-143">onboardingUrl</span></span>|<span data-ttu-id="be43f-144">String</span><span class="sxs-lookup"><span data-stu-id="be43f-144">String</span></span>|<span data-ttu-id="be43f-145">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="be43f-145">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="be43f-146">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="be43f-146">onboardingStatus</span></span>|[<span data-ttu-id="be43f-147">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="be43f-147">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="be43f-148">TBD。</span><span class="sxs-lookup"><span data-stu-id="be43f-148">TBD.</span></span> <span data-ttu-id="be43f-149">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="be43f-149">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="be43f-150">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="be43f-150">lastConnectionDateTime</span></span>|<span data-ttu-id="be43f-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be43f-151">DateTimeOffset</span></span>|<span data-ttu-id="be43f-152">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="be43f-152">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be43f-153">关系</span><span class="sxs-lookup"><span data-stu-id="be43f-153">Relationships</span></span>
<span data-ttu-id="be43f-154">无</span><span class="sxs-lookup"><span data-stu-id="be43f-154">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="be43f-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be43f-155">JSON Representation</span></span>
<span data-ttu-id="be43f-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be43f-156">Here is a JSON representation of the resource.</span></span>
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






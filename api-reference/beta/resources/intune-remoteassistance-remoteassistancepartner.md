---
title: remoteAssistancePartner 资源类型
description: remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b0bdbffc33358770b43ac67dcb67d9acea7655f0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407933"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="4c5ae-103">remoteAssistancePartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c5ae-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="4c5ae-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4c5ae-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c5ae-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c5ae-107">remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-107">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="4c5ae-108">方法</span><span class="sxs-lookup"><span data-stu-id="4c5ae-108">Methods</span></span>
|<span data-ttu-id="4c5ae-109">方法</span><span class="sxs-lookup"><span data-stu-id="4c5ae-109">Method</span></span>|<span data-ttu-id="4c5ae-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4c5ae-110">Return Type</span></span>|<span data-ttu-id="4c5ae-111">说明</span><span class="sxs-lookup"><span data-stu-id="4c5ae-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4c5ae-112">列出 remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="4c5ae-112">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="4c5ae-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c5ae-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="4c5ae-114">列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-114">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="4c5ae-115">获取 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4c5ae-115">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="4c5ae-116">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4c5ae-116">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="4c5ae-117">读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-117">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="4c5ae-118">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4c5ae-118">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="4c5ae-119">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4c5ae-119">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="4c5ae-120">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-120">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="4c5ae-121">删除 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4c5ae-121">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="4c5ae-122">无</span><span class="sxs-lookup"><span data-stu-id="4c5ae-122">None</span></span>|<span data-ttu-id="4c5ae-123">删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-123">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="4c5ae-124">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4c5ae-124">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="4c5ae-125">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4c5ae-125">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="4c5ae-126">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-126">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="4c5ae-127">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="4c5ae-127">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="4c5ae-128">无</span><span class="sxs-lookup"><span data-stu-id="4c5ae-128">None</span></span>|<span data-ttu-id="4c5ae-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4c5ae-129">Not yet documented</span></span>|
|[<span data-ttu-id="4c5ae-130">断开连接操作</span><span class="sxs-lookup"><span data-stu-id="4c5ae-130">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="4c5ae-131">无</span><span class="sxs-lookup"><span data-stu-id="4c5ae-131">None</span></span>|<span data-ttu-id="4c5ae-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4c5ae-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="4c5ae-133">属性</span><span class="sxs-lookup"><span data-stu-id="4c5ae-133">Properties</span></span>
|<span data-ttu-id="4c5ae-134">属性</span><span class="sxs-lookup"><span data-stu-id="4c5ae-134">Property</span></span>|<span data-ttu-id="4c5ae-135">类型</span><span class="sxs-lookup"><span data-stu-id="4c5ae-135">Type</span></span>|<span data-ttu-id="4c5ae-136">说明</span><span class="sxs-lookup"><span data-stu-id="4c5ae-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c5ae-137">id</span><span class="sxs-lookup"><span data-stu-id="4c5ae-137">id</span></span>|<span data-ttu-id="4c5ae-138">String</span><span class="sxs-lookup"><span data-stu-id="4c5ae-138">String</span></span>|<span data-ttu-id="4c5ae-139">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-139">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="4c5ae-140">displayName</span><span class="sxs-lookup"><span data-stu-id="4c5ae-140">displayName</span></span>|<span data-ttu-id="4c5ae-141">String</span><span class="sxs-lookup"><span data-stu-id="4c5ae-141">String</span></span>|<span data-ttu-id="4c5ae-142">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-142">Display name of the partner.</span></span>|
|<span data-ttu-id="4c5ae-143">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="4c5ae-143">onboardingUrl</span></span>|<span data-ttu-id="4c5ae-144">String</span><span class="sxs-lookup"><span data-stu-id="4c5ae-144">String</span></span>|<span data-ttu-id="4c5ae-145">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-145">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="4c5ae-146">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="4c5ae-146">onboardingStatus</span></span>|[<span data-ttu-id="4c5ae-147">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="4c5ae-147">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="4c5ae-148">TBD。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-148">TBD.</span></span> <span data-ttu-id="4c5ae-149">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-149">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="4c5ae-150">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="4c5ae-150">lastConnectionDateTime</span></span>|<span data-ttu-id="4c5ae-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c5ae-151">DateTimeOffset</span></span>|<span data-ttu-id="4c5ae-152">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-152">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c5ae-153">关系</span><span class="sxs-lookup"><span data-stu-id="4c5ae-153">Relationships</span></span>
<span data-ttu-id="4c5ae-154">无</span><span class="sxs-lookup"><span data-stu-id="4c5ae-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c5ae-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c5ae-155">JSON Representation</span></span>
<span data-ttu-id="4c5ae-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c5ae-156">Here is a JSON representation of the resource.</span></span>
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





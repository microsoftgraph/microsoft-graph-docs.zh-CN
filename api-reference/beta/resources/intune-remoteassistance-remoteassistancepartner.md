---
title: remoteAssistancePartner 资源类型
description: RemoteAssistPartner 资源表示给定的远程协助合作伙伴服务的元数据和状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6a71d05d044c3b7e918313643029f738fac54317
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308175"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="fd204-103">remoteAssistancePartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd204-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="fd204-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fd204-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd204-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd204-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd204-106">RemoteAssistPartner 资源表示给定的远程协助合作伙伴服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="fd204-106">RemoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="fd204-107">方法</span><span class="sxs-lookup"><span data-stu-id="fd204-107">Methods</span></span>
|<span data-ttu-id="fd204-108">方法</span><span class="sxs-lookup"><span data-stu-id="fd204-108">Method</span></span>|<span data-ttu-id="fd204-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="fd204-109">Return Type</span></span>|<span data-ttu-id="fd204-110">说明</span><span class="sxs-lookup"><span data-stu-id="fd204-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fd204-111">列出 remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="fd204-111">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="fd204-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd204-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="fd204-113">列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fd204-113">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="fd204-114">获取 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fd204-114">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="fd204-115">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fd204-115">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="fd204-116">读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fd204-116">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="fd204-117">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fd204-117">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="fd204-118">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fd204-118">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="fd204-119">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fd204-119">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="fd204-120">删除 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fd204-120">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="fd204-121">无</span><span class="sxs-lookup"><span data-stu-id="fd204-121">None</span></span>|<span data-ttu-id="fd204-122">删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。</span><span class="sxs-lookup"><span data-stu-id="fd204-122">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="fd204-123">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fd204-123">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="fd204-124">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="fd204-124">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="fd204-125">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fd204-125">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="fd204-126">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="fd204-126">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="fd204-127">无</span><span class="sxs-lookup"><span data-stu-id="fd204-127">None</span></span>|<span data-ttu-id="fd204-128">启动 "加入" 的请求。</span><span class="sxs-lookup"><span data-stu-id="fd204-128">A request to start onboarding.</span></span>  <span data-ttu-id="fd204-129">必须与相应的 TeamViewer 帐户信息结合使用</span><span class="sxs-lookup"><span data-stu-id="fd204-129">Must be coupled with the appropriate TeamViewer account information</span></span>|
|[<span data-ttu-id="fd204-130">断开连接操作</span><span class="sxs-lookup"><span data-stu-id="fd204-130">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="fd204-131">无</span><span class="sxs-lookup"><span data-stu-id="fd204-131">None</span></span>|<span data-ttu-id="fd204-132">请求删除活动的 TeamViewer 连接器</span><span class="sxs-lookup"><span data-stu-id="fd204-132">A request to remove the active TeamViewer connector</span></span>|

## <a name="properties"></a><span data-ttu-id="fd204-133">属性</span><span class="sxs-lookup"><span data-stu-id="fd204-133">Properties</span></span>
|<span data-ttu-id="fd204-134">属性</span><span class="sxs-lookup"><span data-stu-id="fd204-134">Property</span></span>|<span data-ttu-id="fd204-135">类型</span><span class="sxs-lookup"><span data-stu-id="fd204-135">Type</span></span>|<span data-ttu-id="fd204-136">说明</span><span class="sxs-lookup"><span data-stu-id="fd204-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd204-137">id</span><span class="sxs-lookup"><span data-stu-id="fd204-137">id</span></span>|<span data-ttu-id="fd204-138">String</span><span class="sxs-lookup"><span data-stu-id="fd204-138">String</span></span>|<span data-ttu-id="fd204-139">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fd204-139">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="fd204-140">displayName</span><span class="sxs-lookup"><span data-stu-id="fd204-140">displayName</span></span>|<span data-ttu-id="fd204-141">字符串</span><span class="sxs-lookup"><span data-stu-id="fd204-141">String</span></span>|<span data-ttu-id="fd204-142">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fd204-142">Display name of the partner.</span></span>|
|<span data-ttu-id="fd204-143">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="fd204-143">onboardingUrl</span></span>|<span data-ttu-id="fd204-144">String</span><span class="sxs-lookup"><span data-stu-id="fd204-144">String</span></span>|<span data-ttu-id="fd204-145">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="fd204-145">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="fd204-146">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="fd204-146">onboardingStatus</span></span>|[<span data-ttu-id="fd204-147">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="fd204-147">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="fd204-148">当前 TeamViewer 连接器状态的友好说明。</span><span class="sxs-lookup"><span data-stu-id="fd204-148">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="fd204-149">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="fd204-149">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="fd204-150">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="fd204-150">lastConnectionDateTime</span></span>|<span data-ttu-id="fd204-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd204-151">DateTimeOffset</span></span>|<span data-ttu-id="fd204-152">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="fd204-152">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd204-153">关系</span><span class="sxs-lookup"><span data-stu-id="fd204-153">Relationships</span></span>
<span data-ttu-id="fd204-154">无</span><span class="sxs-lookup"><span data-stu-id="fd204-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd204-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd204-155">JSON Representation</span></span>
<span data-ttu-id="fd204-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd204-156">Here is a JSON representation of the resource.</span></span>
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




---
title: remoteAssistancePartner 资源类型
description: RemoteAssistPartner 资源表示给定的远程协助合作伙伴服务的元数据和状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3343d0e9d68c76db91f1153704176d70b06a7483
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566302"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="2fcdd-103">remoteAssistancePartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="2fcdd-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="2fcdd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fcdd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fcdd-106">RemoteAssistPartner 资源表示给定的远程协助合作伙伴服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-106">RemoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="2fcdd-107">方法</span><span class="sxs-lookup"><span data-stu-id="2fcdd-107">Methods</span></span>
|<span data-ttu-id="2fcdd-108">方法</span><span class="sxs-lookup"><span data-stu-id="2fcdd-108">Method</span></span>|<span data-ttu-id="2fcdd-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2fcdd-109">Return Type</span></span>|<span data-ttu-id="2fcdd-110">说明</span><span class="sxs-lookup"><span data-stu-id="2fcdd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2fcdd-111">列出 remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="2fcdd-111">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="2fcdd-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2fcdd-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="2fcdd-113">列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-113">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="2fcdd-114">获取 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="2fcdd-114">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="2fcdd-115">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="2fcdd-115">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="2fcdd-116">读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-116">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="2fcdd-117">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="2fcdd-117">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="2fcdd-118">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="2fcdd-118">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="2fcdd-119">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-119">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="2fcdd-120">删除 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="2fcdd-120">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="2fcdd-121">无</span><span class="sxs-lookup"><span data-stu-id="2fcdd-121">None</span></span>|<span data-ttu-id="2fcdd-122">删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-122">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="2fcdd-123">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="2fcdd-123">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="2fcdd-124">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="2fcdd-124">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="2fcdd-125">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-125">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="2fcdd-126">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="2fcdd-126">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="2fcdd-127">无</span><span class="sxs-lookup"><span data-stu-id="2fcdd-127">None</span></span>|<span data-ttu-id="2fcdd-128">启动 "加入" 的请求。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-128">A request to start onboarding.</span></span>  <span data-ttu-id="2fcdd-129">必须与相应的 TeamViewer 帐户信息结合使用</span><span class="sxs-lookup"><span data-stu-id="2fcdd-129">Must be coupled with the appropriate TeamViewer account information</span></span>|
|[<span data-ttu-id="2fcdd-130">断开连接操作</span><span class="sxs-lookup"><span data-stu-id="2fcdd-130">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="2fcdd-131">无</span><span class="sxs-lookup"><span data-stu-id="2fcdd-131">None</span></span>|<span data-ttu-id="2fcdd-132">请求删除活动的 TeamViewer 连接器</span><span class="sxs-lookup"><span data-stu-id="2fcdd-132">A request to remove the active TeamViewer connector</span></span>|

## <a name="properties"></a><span data-ttu-id="2fcdd-133">属性</span><span class="sxs-lookup"><span data-stu-id="2fcdd-133">Properties</span></span>
|<span data-ttu-id="2fcdd-134">属性</span><span class="sxs-lookup"><span data-stu-id="2fcdd-134">Property</span></span>|<span data-ttu-id="2fcdd-135">类型</span><span class="sxs-lookup"><span data-stu-id="2fcdd-135">Type</span></span>|<span data-ttu-id="2fcdd-136">说明</span><span class="sxs-lookup"><span data-stu-id="2fcdd-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fcdd-137">id</span><span class="sxs-lookup"><span data-stu-id="2fcdd-137">id</span></span>|<span data-ttu-id="2fcdd-138">String</span><span class="sxs-lookup"><span data-stu-id="2fcdd-138">String</span></span>|<span data-ttu-id="2fcdd-139">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-139">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="2fcdd-140">displayName</span><span class="sxs-lookup"><span data-stu-id="2fcdd-140">displayName</span></span>|<span data-ttu-id="2fcdd-141">字符串</span><span class="sxs-lookup"><span data-stu-id="2fcdd-141">String</span></span>|<span data-ttu-id="2fcdd-142">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-142">Display name of the partner.</span></span>|
|<span data-ttu-id="2fcdd-143">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="2fcdd-143">onboardingUrl</span></span>|<span data-ttu-id="2fcdd-144">String</span><span class="sxs-lookup"><span data-stu-id="2fcdd-144">String</span></span>|<span data-ttu-id="2fcdd-145">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-145">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="2fcdd-146">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="2fcdd-146">onboardingStatus</span></span>|[<span data-ttu-id="2fcdd-147">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="2fcdd-147">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="2fcdd-148">当前 TeamViewer 连接器状态的友好说明。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-148">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="2fcdd-149">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-149">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="2fcdd-150">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="2fcdd-150">lastConnectionDateTime</span></span>|<span data-ttu-id="2fcdd-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fcdd-151">DateTimeOffset</span></span>|<span data-ttu-id="2fcdd-152">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-152">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fcdd-153">关系</span><span class="sxs-lookup"><span data-stu-id="2fcdd-153">Relationships</span></span>
<span data-ttu-id="2fcdd-154">无</span><span class="sxs-lookup"><span data-stu-id="2fcdd-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fcdd-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2fcdd-155">JSON Representation</span></span>
<span data-ttu-id="2fcdd-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2fcdd-156">Here is a JSON representation of the resource.</span></span>
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






---
title: remoteAssistancePartner 资源类型
description: RemoteAssistPartner 资源表示给定的远程协助合作伙伴服务的元数据和状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b85cd11112045df5ff2babfee5f8b51dec57c0d6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772809"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="91a77-103">remoteAssistancePartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="91a77-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="91a77-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="91a77-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91a77-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="91a77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91a77-106">RemoteAssistPartner 资源表示给定的远程协助合作伙伴服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="91a77-106">RemoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="91a77-107">方法</span><span class="sxs-lookup"><span data-stu-id="91a77-107">Methods</span></span>
|<span data-ttu-id="91a77-108">方法</span><span class="sxs-lookup"><span data-stu-id="91a77-108">Method</span></span>|<span data-ttu-id="91a77-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="91a77-109">Return Type</span></span>|<span data-ttu-id="91a77-110">说明</span><span class="sxs-lookup"><span data-stu-id="91a77-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="91a77-111">列出 remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="91a77-111">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="91a77-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="91a77-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="91a77-113">列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="91a77-113">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="91a77-114">获取 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="91a77-114">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="91a77-115">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="91a77-115">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="91a77-116">读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="91a77-116">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="91a77-117">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="91a77-117">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="91a77-118">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="91a77-118">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="91a77-119">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="91a77-119">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="91a77-120">删除 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="91a77-120">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="91a77-121">无</span><span class="sxs-lookup"><span data-stu-id="91a77-121">None</span></span>|<span data-ttu-id="91a77-122">删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。</span><span class="sxs-lookup"><span data-stu-id="91a77-122">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="91a77-123">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="91a77-123">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="91a77-124">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="91a77-124">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="91a77-125">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="91a77-125">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="91a77-126">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="91a77-126">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="91a77-127">None</span><span class="sxs-lookup"><span data-stu-id="91a77-127">None</span></span>|<span data-ttu-id="91a77-128">启动 "加入" 的请求。</span><span class="sxs-lookup"><span data-stu-id="91a77-128">A request to start onboarding.</span></span>  <span data-ttu-id="91a77-129">必须与相应的 TeamViewer 帐户信息结合使用</span><span class="sxs-lookup"><span data-stu-id="91a77-129">Must be coupled with the appropriate TeamViewer account information</span></span>|
|[<span data-ttu-id="91a77-130">断开连接操作</span><span class="sxs-lookup"><span data-stu-id="91a77-130">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="91a77-131">无</span><span class="sxs-lookup"><span data-stu-id="91a77-131">None</span></span>|<span data-ttu-id="91a77-132">请求删除活动的 TeamViewer 连接器</span><span class="sxs-lookup"><span data-stu-id="91a77-132">A request to remove the active TeamViewer connector</span></span>|

## <a name="properties"></a><span data-ttu-id="91a77-133">属性</span><span class="sxs-lookup"><span data-stu-id="91a77-133">Properties</span></span>
|<span data-ttu-id="91a77-134">属性</span><span class="sxs-lookup"><span data-stu-id="91a77-134">Property</span></span>|<span data-ttu-id="91a77-135">类型</span><span class="sxs-lookup"><span data-stu-id="91a77-135">Type</span></span>|<span data-ttu-id="91a77-136">说明</span><span class="sxs-lookup"><span data-stu-id="91a77-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91a77-137">id</span><span class="sxs-lookup"><span data-stu-id="91a77-137">id</span></span>|<span data-ttu-id="91a77-138">String</span><span class="sxs-lookup"><span data-stu-id="91a77-138">String</span></span>|<span data-ttu-id="91a77-139">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="91a77-139">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="91a77-140">displayName</span><span class="sxs-lookup"><span data-stu-id="91a77-140">displayName</span></span>|<span data-ttu-id="91a77-141">字符串</span><span class="sxs-lookup"><span data-stu-id="91a77-141">String</span></span>|<span data-ttu-id="91a77-142">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="91a77-142">Display name of the partner.</span></span>|
|<span data-ttu-id="91a77-143">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="91a77-143">onboardingUrl</span></span>|<span data-ttu-id="91a77-144">String</span><span class="sxs-lookup"><span data-stu-id="91a77-144">String</span></span>|<span data-ttu-id="91a77-145">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="91a77-145">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="91a77-146">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="91a77-146">onboardingStatus</span></span>|[<span data-ttu-id="91a77-147">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="91a77-147">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="91a77-148">当前 TeamViewer 连接器状态的友好说明。</span><span class="sxs-lookup"><span data-stu-id="91a77-148">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="91a77-149">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="91a77-149">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="91a77-150">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="91a77-150">lastConnectionDateTime</span></span>|<span data-ttu-id="91a77-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91a77-151">DateTimeOffset</span></span>|<span data-ttu-id="91a77-152">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="91a77-152">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91a77-153">关系</span><span class="sxs-lookup"><span data-stu-id="91a77-153">Relationships</span></span>
<span data-ttu-id="91a77-154">无</span><span class="sxs-lookup"><span data-stu-id="91a77-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91a77-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91a77-155">JSON Representation</span></span>
<span data-ttu-id="91a77-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91a77-156">Here is a JSON representation of the resource.</span></span>
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




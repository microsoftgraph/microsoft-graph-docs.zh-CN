---
title: remoteAssistancePartner 资源类型
description: RemoteAssistPartner 资源表示给定的远程协助合作伙伴服务的元数据和状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ed8c9a2d8de2aa315e8b03f1ce6f9ef4b7586a97
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523812"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="4f2d9-103">remoteAssistancePartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f2d9-103">remoteAssistancePartner resource type</span></span>

<span data-ttu-id="4f2d9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4f2d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f2d9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f2d9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f2d9-107">RemoteAssistPartner 资源表示给定的远程协助合作伙伴服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-107">RemoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="4f2d9-108">方法</span><span class="sxs-lookup"><span data-stu-id="4f2d9-108">Methods</span></span>
|<span data-ttu-id="4f2d9-109">方法</span><span class="sxs-lookup"><span data-stu-id="4f2d9-109">Method</span></span>|<span data-ttu-id="4f2d9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f2d9-110">Return Type</span></span>|<span data-ttu-id="4f2d9-111">说明</span><span class="sxs-lookup"><span data-stu-id="4f2d9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4f2d9-112">列出 remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="4f2d9-112">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="4f2d9-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f2d9-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="4f2d9-114">列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-114">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="4f2d9-115">获取 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4f2d9-115">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="4f2d9-116">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4f2d9-116">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="4f2d9-117">读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-117">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="4f2d9-118">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4f2d9-118">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="4f2d9-119">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4f2d9-119">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="4f2d9-120">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-120">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="4f2d9-121">删除 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4f2d9-121">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="4f2d9-122">无</span><span class="sxs-lookup"><span data-stu-id="4f2d9-122">None</span></span>|<span data-ttu-id="4f2d9-123">删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-123">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="4f2d9-124">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4f2d9-124">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="4f2d9-125">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="4f2d9-125">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="4f2d9-126">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-126">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="4f2d9-127">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="4f2d9-127">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="4f2d9-128">无</span><span class="sxs-lookup"><span data-stu-id="4f2d9-128">None</span></span>|<span data-ttu-id="4f2d9-129">启动 "加入" 的请求。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-129">A request to start onboarding.</span></span>  <span data-ttu-id="4f2d9-130">必须与相应的 TeamViewer 帐户信息结合使用</span><span class="sxs-lookup"><span data-stu-id="4f2d9-130">Must be coupled with the appropriate TeamViewer account information</span></span>|
|[<span data-ttu-id="4f2d9-131">断开连接操作</span><span class="sxs-lookup"><span data-stu-id="4f2d9-131">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="4f2d9-132">无</span><span class="sxs-lookup"><span data-stu-id="4f2d9-132">None</span></span>|<span data-ttu-id="4f2d9-133">请求删除活动的 TeamViewer 连接器</span><span class="sxs-lookup"><span data-stu-id="4f2d9-133">A request to remove the active TeamViewer connector</span></span>|

## <a name="properties"></a><span data-ttu-id="4f2d9-134">属性</span><span class="sxs-lookup"><span data-stu-id="4f2d9-134">Properties</span></span>
|<span data-ttu-id="4f2d9-135">属性</span><span class="sxs-lookup"><span data-stu-id="4f2d9-135">Property</span></span>|<span data-ttu-id="4f2d9-136">类型</span><span class="sxs-lookup"><span data-stu-id="4f2d9-136">Type</span></span>|<span data-ttu-id="4f2d9-137">说明</span><span class="sxs-lookup"><span data-stu-id="4f2d9-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f2d9-138">id</span><span class="sxs-lookup"><span data-stu-id="4f2d9-138">id</span></span>|<span data-ttu-id="4f2d9-139">String</span><span class="sxs-lookup"><span data-stu-id="4f2d9-139">String</span></span>|<span data-ttu-id="4f2d9-140">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-140">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="4f2d9-141">displayName</span><span class="sxs-lookup"><span data-stu-id="4f2d9-141">displayName</span></span>|<span data-ttu-id="4f2d9-142">字符串</span><span class="sxs-lookup"><span data-stu-id="4f2d9-142">String</span></span>|<span data-ttu-id="4f2d9-143">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-143">Display name of the partner.</span></span>|
|<span data-ttu-id="4f2d9-144">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="4f2d9-144">onboardingUrl</span></span>|<span data-ttu-id="4f2d9-145">String</span><span class="sxs-lookup"><span data-stu-id="4f2d9-145">String</span></span>|<span data-ttu-id="4f2d9-146">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-146">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="4f2d9-147">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="4f2d9-147">onboardingStatus</span></span>|[<span data-ttu-id="4f2d9-148">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="4f2d9-148">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="4f2d9-149">当前 TeamViewer 连接器状态的友好说明。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-149">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="4f2d9-150">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-150">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="4f2d9-151">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="4f2d9-151">lastConnectionDateTime</span></span>|<span data-ttu-id="4f2d9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f2d9-152">DateTimeOffset</span></span>|<span data-ttu-id="4f2d9-153">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-153">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f2d9-154">关系</span><span class="sxs-lookup"><span data-stu-id="4f2d9-154">Relationships</span></span>
<span data-ttu-id="4f2d9-155">无</span><span class="sxs-lookup"><span data-stu-id="4f2d9-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f2d9-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f2d9-156">JSON Representation</span></span>
<span data-ttu-id="4f2d9-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f2d9-157">Here is a JSON representation of the resource.</span></span>
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




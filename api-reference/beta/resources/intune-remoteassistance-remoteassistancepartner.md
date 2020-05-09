---
title: remoteAssistancePartner 资源类型
description: RemoteAssistPartner 资源表示给定的远程协助合作伙伴服务的元数据和状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d82d63df7dd584d75410097d484b0187f98bb9f6
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44176130"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="ddadb-103">remoteAssistancePartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="ddadb-103">remoteAssistancePartner resource type</span></span>

<span data-ttu-id="ddadb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddadb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddadb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ddadb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddadb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ddadb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddadb-107">RemoteAssistPartner 资源表示给定的远程协助合作伙伴服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="ddadb-107">RemoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="ddadb-108">方法</span><span class="sxs-lookup"><span data-stu-id="ddadb-108">Methods</span></span>
|<span data-ttu-id="ddadb-109">方法</span><span class="sxs-lookup"><span data-stu-id="ddadb-109">Method</span></span>|<span data-ttu-id="ddadb-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ddadb-110">Return Type</span></span>|<span data-ttu-id="ddadb-111">说明</span><span class="sxs-lookup"><span data-stu-id="ddadb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ddadb-112">列出 remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="ddadb-112">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="ddadb-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ddadb-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="ddadb-114">列出 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ddadb-114">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="ddadb-115">获取 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ddadb-115">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="ddadb-116">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ddadb-116">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="ddadb-117">读取 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ddadb-117">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="ddadb-118">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ddadb-118">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="ddadb-119">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ddadb-119">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="ddadb-120">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ddadb-120">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="ddadb-121">删除 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ddadb-121">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="ddadb-122">无</span><span class="sxs-lookup"><span data-stu-id="ddadb-122">None</span></span>|<span data-ttu-id="ddadb-123">删除 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)。</span><span class="sxs-lookup"><span data-stu-id="ddadb-123">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="ddadb-124">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ddadb-124">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="ddadb-125">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ddadb-125">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="ddadb-126">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ddadb-126">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="ddadb-127">beginOnboarding 操作</span><span class="sxs-lookup"><span data-stu-id="ddadb-127">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="ddadb-128">无</span><span class="sxs-lookup"><span data-stu-id="ddadb-128">None</span></span>|<span data-ttu-id="ddadb-129">启动 "加入" 的请求。</span><span class="sxs-lookup"><span data-stu-id="ddadb-129">A request to start onboarding.</span></span>  <span data-ttu-id="ddadb-130">必须与相应的 TeamViewer 帐户信息结合使用</span><span class="sxs-lookup"><span data-stu-id="ddadb-130">Must be coupled with the appropriate TeamViewer account information</span></span>|
|[<span data-ttu-id="ddadb-131">断开连接操作</span><span class="sxs-lookup"><span data-stu-id="ddadb-131">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="ddadb-132">无</span><span class="sxs-lookup"><span data-stu-id="ddadb-132">None</span></span>|<span data-ttu-id="ddadb-133">请求删除活动的 TeamViewer 连接器</span><span class="sxs-lookup"><span data-stu-id="ddadb-133">A request to remove the active TeamViewer connector</span></span>|

## <a name="properties"></a><span data-ttu-id="ddadb-134">属性</span><span class="sxs-lookup"><span data-stu-id="ddadb-134">Properties</span></span>
|<span data-ttu-id="ddadb-135">属性</span><span class="sxs-lookup"><span data-stu-id="ddadb-135">Property</span></span>|<span data-ttu-id="ddadb-136">类型</span><span class="sxs-lookup"><span data-stu-id="ddadb-136">Type</span></span>|<span data-ttu-id="ddadb-137">说明</span><span class="sxs-lookup"><span data-stu-id="ddadb-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddadb-138">id</span><span class="sxs-lookup"><span data-stu-id="ddadb-138">id</span></span>|<span data-ttu-id="ddadb-139">字符串</span><span class="sxs-lookup"><span data-stu-id="ddadb-139">String</span></span>|<span data-ttu-id="ddadb-140">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ddadb-140">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="ddadb-141">displayName</span><span class="sxs-lookup"><span data-stu-id="ddadb-141">displayName</span></span>|<span data-ttu-id="ddadb-142">字符串</span><span class="sxs-lookup"><span data-stu-id="ddadb-142">String</span></span>|<span data-ttu-id="ddadb-143">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ddadb-143">Display name of the partner.</span></span>|
|<span data-ttu-id="ddadb-144">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="ddadb-144">onboardingUrl</span></span>|<span data-ttu-id="ddadb-145">String</span><span class="sxs-lookup"><span data-stu-id="ddadb-145">String</span></span>|<span data-ttu-id="ddadb-146">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="ddadb-146">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="ddadb-147">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="ddadb-147">onboardingStatus</span></span>|[<span data-ttu-id="ddadb-148">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="ddadb-148">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="ddadb-149">当前 TeamViewer 连接器状态的友好说明。</span><span class="sxs-lookup"><span data-stu-id="ddadb-149">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="ddadb-150">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="ddadb-150">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="ddadb-151">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="ddadb-151">lastConnectionDateTime</span></span>|<span data-ttu-id="ddadb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddadb-152">DateTimeOffset</span></span>|<span data-ttu-id="ddadb-153">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="ddadb-153">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddadb-154">关系</span><span class="sxs-lookup"><span data-stu-id="ddadb-154">Relationships</span></span>
<span data-ttu-id="ddadb-155">无</span><span class="sxs-lookup"><span data-stu-id="ddadb-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddadb-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ddadb-156">JSON Representation</span></span>
<span data-ttu-id="ddadb-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddadb-157">Here is a JSON representation of the resource.</span></span>
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




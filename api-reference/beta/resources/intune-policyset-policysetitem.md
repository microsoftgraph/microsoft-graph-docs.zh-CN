---
title: policySetItem 资源类型
description: 包含用于 PolicySet 项目的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 530dd10960eacd0ded5c5c8d9340469c66020e8c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993411"
---
# <a name="policysetitem-resource-type"></a><span data-ttu-id="eb279-103">policySetItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb279-103">policySetItem resource type</span></span>

<span data-ttu-id="eb279-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb279-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb279-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eb279-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb279-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb279-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb279-107">包含用于 PolicySet 项目的属性的类。</span><span class="sxs-lookup"><span data-stu-id="eb279-107">A class containing the properties used for PolicySet Item.</span></span>

## <a name="methods"></a><span data-ttu-id="eb279-108">方法</span><span class="sxs-lookup"><span data-stu-id="eb279-108">Methods</span></span>
|<span data-ttu-id="eb279-109">方法</span><span class="sxs-lookup"><span data-stu-id="eb279-109">Method</span></span>|<span data-ttu-id="eb279-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="eb279-110">Return Type</span></span>|<span data-ttu-id="eb279-111">说明</span><span class="sxs-lookup"><span data-stu-id="eb279-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eb279-112">列出 policySetItems</span><span class="sxs-lookup"><span data-stu-id="eb279-112">List policySetItems</span></span>](../api/intune-policyset-policysetitem-list.md)|<span data-ttu-id="eb279-113">[policySetItem](../resources/intune-policyset-policysetitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb279-113">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="eb279-114">列出 [policySetItem](../resources/intune-policyset-policysetitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eb279-114">List properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) objects.</span></span>|
|[<span data-ttu-id="eb279-115">获取 policySetItem</span><span class="sxs-lookup"><span data-stu-id="eb279-115">Get policySetItem</span></span>](../api/intune-policyset-policysetitem-get.md)|[<span data-ttu-id="eb279-116">policySetItem</span><span class="sxs-lookup"><span data-stu-id="eb279-116">policySetItem</span></span>](../resources/intune-policyset-policysetitem.md)|<span data-ttu-id="eb279-117">读取 [policySetItem](../resources/intune-policyset-policysetitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eb279-117">Read properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="eb279-118">属性</span><span class="sxs-lookup"><span data-stu-id="eb279-118">Properties</span></span>
|<span data-ttu-id="eb279-119">属性</span><span class="sxs-lookup"><span data-stu-id="eb279-119">Property</span></span>|<span data-ttu-id="eb279-120">类型</span><span class="sxs-lookup"><span data-stu-id="eb279-120">Type</span></span>|<span data-ttu-id="eb279-121">说明</span><span class="sxs-lookup"><span data-stu-id="eb279-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb279-122">id</span><span class="sxs-lookup"><span data-stu-id="eb279-122">id</span></span>|<span data-ttu-id="eb279-123">String</span><span class="sxs-lookup"><span data-stu-id="eb279-123">String</span></span>|<span data-ttu-id="eb279-124">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="eb279-124">Key of the MobileAppPolicySetItem.</span></span>|
|<span data-ttu-id="eb279-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb279-125">createdDateTime</span></span>|<span data-ttu-id="eb279-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb279-126">DateTimeOffset</span></span>|<span data-ttu-id="eb279-127">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="eb279-127">Creation time of the PolicySetItem.</span></span>|
|<span data-ttu-id="eb279-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb279-128">lastModifiedDateTime</span></span>|<span data-ttu-id="eb279-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb279-129">DateTimeOffset</span></span>|<span data-ttu-id="eb279-130">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="eb279-130">Last modified time of the PolicySetItem.</span></span>|
|<span data-ttu-id="eb279-131">payloadId</span><span class="sxs-lookup"><span data-stu-id="eb279-131">payloadId</span></span>|<span data-ttu-id="eb279-132">String</span><span class="sxs-lookup"><span data-stu-id="eb279-132">String</span></span>|<span data-ttu-id="eb279-133">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="eb279-133">PayloadId of the PolicySetItem.</span></span>|
|<span data-ttu-id="eb279-134">itemType</span><span class="sxs-lookup"><span data-stu-id="eb279-134">itemType</span></span>|<span data-ttu-id="eb279-135">String</span><span class="sxs-lookup"><span data-stu-id="eb279-135">String</span></span>|<span data-ttu-id="eb279-136">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="eb279-136">policySetType of the PolicySetItem.</span></span>|
|<span data-ttu-id="eb279-137">displayName</span><span class="sxs-lookup"><span data-stu-id="eb279-137">displayName</span></span>|<span data-ttu-id="eb279-138">String</span><span class="sxs-lookup"><span data-stu-id="eb279-138">String</span></span>|<span data-ttu-id="eb279-139">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="eb279-139">DisplayName of the PolicySetItem.</span></span>|
|<span data-ttu-id="eb279-140">状态</span><span class="sxs-lookup"><span data-stu-id="eb279-140">status</span></span>|[<span data-ttu-id="eb279-141">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="eb279-141">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="eb279-142">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="eb279-142">Status of the PolicySetItem.</span></span> <span data-ttu-id="eb279-143">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="eb279-143">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="eb279-144">errorCode</span><span class="sxs-lookup"><span data-stu-id="eb279-144">errorCode</span></span>|[<span data-ttu-id="eb279-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="eb279-145">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="eb279-146">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="eb279-146">Error code if any occured.</span></span> <span data-ttu-id="eb279-147">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="eb279-147">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="eb279-148">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="eb279-148">guidedDeploymentTags</span></span>|<span data-ttu-id="eb279-149">String collection</span><span class="sxs-lookup"><span data-stu-id="eb279-149">String collection</span></span>|<span data-ttu-id="eb279-150">引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="eb279-150">Tags of the guided deployment</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb279-151">关系</span><span class="sxs-lookup"><span data-stu-id="eb279-151">Relationships</span></span>
<span data-ttu-id="eb279-152">无</span><span class="sxs-lookup"><span data-stu-id="eb279-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb279-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb279-153">JSON Representation</span></span>
<span data-ttu-id="eb279-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb279-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ]
}
```







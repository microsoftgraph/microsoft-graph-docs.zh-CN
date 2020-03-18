---
title: policySetItem 资源类型
description: 包含用于 PolicySet 项目的属性的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 98000e00ad90938bc3835b9ba3becb047920fd0a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42729106"
---
# <a name="policysetitem-resource-type"></a><span data-ttu-id="21673-103">policySetItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="21673-103">policySetItem resource type</span></span>

> <span data-ttu-id="21673-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="21673-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21673-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21673-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21673-106">包含用于 PolicySet 项目的属性的类。</span><span class="sxs-lookup"><span data-stu-id="21673-106">A class containing the properties used for PolicySet Item.</span></span>

## <a name="methods"></a><span data-ttu-id="21673-107">方法</span><span class="sxs-lookup"><span data-stu-id="21673-107">Methods</span></span>
|<span data-ttu-id="21673-108">方法</span><span class="sxs-lookup"><span data-stu-id="21673-108">Method</span></span>|<span data-ttu-id="21673-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="21673-109">Return Type</span></span>|<span data-ttu-id="21673-110">说明</span><span class="sxs-lookup"><span data-stu-id="21673-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="21673-111">列出 policySetItems</span><span class="sxs-lookup"><span data-stu-id="21673-111">List policySetItems</span></span>](../api/intune-policyset-policysetitem-list.md)|<span data-ttu-id="21673-112">[policySetItem](../resources/intune-policyset-policysetitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="21673-112">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="21673-113">列出[policySetItem](../resources/intune-policyset-policysetitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="21673-113">List properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) objects.</span></span>|
|[<span data-ttu-id="21673-114">获取 policySetItem</span><span class="sxs-lookup"><span data-stu-id="21673-114">Get policySetItem</span></span>](../api/intune-policyset-policysetitem-get.md)|[<span data-ttu-id="21673-115">policySetItem</span><span class="sxs-lookup"><span data-stu-id="21673-115">policySetItem</span></span>](../resources/intune-policyset-policysetitem.md)|<span data-ttu-id="21673-116">读取[policySetItem](../resources/intune-policyset-policysetitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="21673-116">Read properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="21673-117">属性</span><span class="sxs-lookup"><span data-stu-id="21673-117">Properties</span></span>
|<span data-ttu-id="21673-118">属性</span><span class="sxs-lookup"><span data-stu-id="21673-118">Property</span></span>|<span data-ttu-id="21673-119">类型</span><span class="sxs-lookup"><span data-stu-id="21673-119">Type</span></span>|<span data-ttu-id="21673-120">说明</span><span class="sxs-lookup"><span data-stu-id="21673-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21673-121">id</span><span class="sxs-lookup"><span data-stu-id="21673-121">id</span></span>|<span data-ttu-id="21673-122">String</span><span class="sxs-lookup"><span data-stu-id="21673-122">String</span></span>|<span data-ttu-id="21673-123">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="21673-123">Key of the MobileAppPolicySetItem.</span></span>|
|<span data-ttu-id="21673-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21673-124">createdDateTime</span></span>|<span data-ttu-id="21673-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21673-125">DateTimeOffset</span></span>|<span data-ttu-id="21673-126">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="21673-126">Creation time of the PolicySetItem.</span></span>|
|<span data-ttu-id="21673-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21673-127">lastModifiedDateTime</span></span>|<span data-ttu-id="21673-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21673-128">DateTimeOffset</span></span>|<span data-ttu-id="21673-129">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="21673-129">Last modified time of the PolicySetItem.</span></span>|
|<span data-ttu-id="21673-130">payloadId</span><span class="sxs-lookup"><span data-stu-id="21673-130">payloadId</span></span>|<span data-ttu-id="21673-131">String</span><span class="sxs-lookup"><span data-stu-id="21673-131">String</span></span>|<span data-ttu-id="21673-132">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="21673-132">PayloadId of the PolicySetItem.</span></span>|
|<span data-ttu-id="21673-133">itemType</span><span class="sxs-lookup"><span data-stu-id="21673-133">itemType</span></span>|<span data-ttu-id="21673-134">String</span><span class="sxs-lookup"><span data-stu-id="21673-134">String</span></span>|<span data-ttu-id="21673-135">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="21673-135">policySetType of the PolicySetItem.</span></span>|
|<span data-ttu-id="21673-136">displayName</span><span class="sxs-lookup"><span data-stu-id="21673-136">displayName</span></span>|<span data-ttu-id="21673-137">String</span><span class="sxs-lookup"><span data-stu-id="21673-137">String</span></span>|<span data-ttu-id="21673-138">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="21673-138">DisplayName of the PolicySetItem.</span></span>|
|<span data-ttu-id="21673-139">状态</span><span class="sxs-lookup"><span data-stu-id="21673-139">status</span></span>|[<span data-ttu-id="21673-140">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="21673-140">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="21673-141">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="21673-141">Status of the PolicySetItem.</span></span> <span data-ttu-id="21673-142">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="21673-142">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="21673-143">errorCode</span><span class="sxs-lookup"><span data-stu-id="21673-143">errorCode</span></span>|[<span data-ttu-id="21673-144">errorCode</span><span class="sxs-lookup"><span data-stu-id="21673-144">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="21673-145">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="21673-145">Error code if any occured.</span></span> <span data-ttu-id="21673-146">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="21673-146">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="21673-147">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="21673-147">guidedDeploymentTags</span></span>|<span data-ttu-id="21673-148">String collection</span><span class="sxs-lookup"><span data-stu-id="21673-148">String collection</span></span>|<span data-ttu-id="21673-149">引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="21673-149">Tags of the guided deployment</span></span>|

## <a name="relationships"></a><span data-ttu-id="21673-150">关系</span><span class="sxs-lookup"><span data-stu-id="21673-150">Relationships</span></span>
<span data-ttu-id="21673-151">无</span><span class="sxs-lookup"><span data-stu-id="21673-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21673-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21673-152">JSON Representation</span></span>
<span data-ttu-id="21673-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21673-153">Here is a JSON representation of the resource.</span></span>
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




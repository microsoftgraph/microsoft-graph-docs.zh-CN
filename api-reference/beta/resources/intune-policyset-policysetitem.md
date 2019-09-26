---
title: policySetItem 资源类型
description: 包含用于 PolicySet 项目的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 11ebd543bf14df00bddd408dcb26400e3e783b6f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199957"
---
# <a name="policysetitem-resource-type"></a><span data-ttu-id="b67ba-103">policySetItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="b67ba-103">policySetItem resource type</span></span>

> <span data-ttu-id="b67ba-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b67ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b67ba-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b67ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b67ba-106">包含用于 PolicySet 项目的属性的类。</span><span class="sxs-lookup"><span data-stu-id="b67ba-106">A class containing the properties used for PolicySet Item.</span></span>

## <a name="methods"></a><span data-ttu-id="b67ba-107">方法</span><span class="sxs-lookup"><span data-stu-id="b67ba-107">Methods</span></span>
|<span data-ttu-id="b67ba-108">方法</span><span class="sxs-lookup"><span data-stu-id="b67ba-108">Method</span></span>|<span data-ttu-id="b67ba-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b67ba-109">Return Type</span></span>|<span data-ttu-id="b67ba-110">说明</span><span class="sxs-lookup"><span data-stu-id="b67ba-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b67ba-111">列出 policySetItems</span><span class="sxs-lookup"><span data-stu-id="b67ba-111">List policySetItems</span></span>](../api/intune-policyset-policysetitem-list.md)|<span data-ttu-id="b67ba-112">[policySetItem](../resources/intune-policyset-policysetitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="b67ba-112">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="b67ba-113">列出[policySetItem](../resources/intune-policyset-policysetitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b67ba-113">List properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) objects.</span></span>|
|[<span data-ttu-id="b67ba-114">获取 policySetItem</span><span class="sxs-lookup"><span data-stu-id="b67ba-114">Get policySetItem</span></span>](../api/intune-policyset-policysetitem-get.md)|[<span data-ttu-id="b67ba-115">policySetItem</span><span class="sxs-lookup"><span data-stu-id="b67ba-115">policySetItem</span></span>](../resources/intune-policyset-policysetitem.md)|<span data-ttu-id="b67ba-116">读取[policySetItem](../resources/intune-policyset-policysetitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b67ba-116">Read properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b67ba-117">属性</span><span class="sxs-lookup"><span data-stu-id="b67ba-117">Properties</span></span>
|<span data-ttu-id="b67ba-118">属性</span><span class="sxs-lookup"><span data-stu-id="b67ba-118">Property</span></span>|<span data-ttu-id="b67ba-119">类型</span><span class="sxs-lookup"><span data-stu-id="b67ba-119">Type</span></span>|<span data-ttu-id="b67ba-120">说明</span><span class="sxs-lookup"><span data-stu-id="b67ba-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b67ba-121">id</span><span class="sxs-lookup"><span data-stu-id="b67ba-121">id</span></span>|<span data-ttu-id="b67ba-122">String</span><span class="sxs-lookup"><span data-stu-id="b67ba-122">String</span></span>|<span data-ttu-id="b67ba-123">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="b67ba-123">Key of the MobileAppPolicySetItem.</span></span>|
|<span data-ttu-id="b67ba-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b67ba-124">createdDateTime</span></span>|<span data-ttu-id="b67ba-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b67ba-125">DateTimeOffset</span></span>|<span data-ttu-id="b67ba-126">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="b67ba-126">Creation time of the PolicySetItem.</span></span>|
|<span data-ttu-id="b67ba-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b67ba-127">lastModifiedDateTime</span></span>|<span data-ttu-id="b67ba-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b67ba-128">DateTimeOffset</span></span>|<span data-ttu-id="b67ba-129">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="b67ba-129">Last modified time of the PolicySetItem.</span></span>|
|<span data-ttu-id="b67ba-130">payloadId</span><span class="sxs-lookup"><span data-stu-id="b67ba-130">payloadId</span></span>|<span data-ttu-id="b67ba-131">String</span><span class="sxs-lookup"><span data-stu-id="b67ba-131">String</span></span>|<span data-ttu-id="b67ba-132">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="b67ba-132">PayloadId of the PolicySetItem.</span></span>|
|<span data-ttu-id="b67ba-133">itemType</span><span class="sxs-lookup"><span data-stu-id="b67ba-133">itemType</span></span>|<span data-ttu-id="b67ba-134">String</span><span class="sxs-lookup"><span data-stu-id="b67ba-134">String</span></span>|<span data-ttu-id="b67ba-135">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="b67ba-135">policySetType of the PolicySetItem.</span></span>|
|<span data-ttu-id="b67ba-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b67ba-136">displayName</span></span>|<span data-ttu-id="b67ba-137">String</span><span class="sxs-lookup"><span data-stu-id="b67ba-137">String</span></span>|<span data-ttu-id="b67ba-138">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="b67ba-138">DisplayName of the PolicySetItem.</span></span>|
|<span data-ttu-id="b67ba-139">status</span><span class="sxs-lookup"><span data-stu-id="b67ba-139">status</span></span>|[<span data-ttu-id="b67ba-140">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="b67ba-140">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="b67ba-141">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="b67ba-141">Status of the PolicySetItem.</span></span> <span data-ttu-id="b67ba-142">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="b67ba-142">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="b67ba-143">errorCode</span><span class="sxs-lookup"><span data-stu-id="b67ba-143">errorCode</span></span>|[<span data-ttu-id="b67ba-144">错误</span><span class="sxs-lookup"><span data-stu-id="b67ba-144">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="b67ba-145">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="b67ba-145">Error code if any occured.</span></span> <span data-ttu-id="b67ba-146">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="b67ba-146">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="b67ba-147">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="b67ba-147">guidedDeploymentTags</span></span>|<span data-ttu-id="b67ba-148">String collection</span><span class="sxs-lookup"><span data-stu-id="b67ba-148">String collection</span></span>|<span data-ttu-id="b67ba-149">引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="b67ba-149">Tags of the guided deployment</span></span>|

## <a name="relationships"></a><span data-ttu-id="b67ba-150">关系</span><span class="sxs-lookup"><span data-stu-id="b67ba-150">Relationships</span></span>
<span data-ttu-id="b67ba-151">无</span><span class="sxs-lookup"><span data-stu-id="b67ba-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b67ba-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b67ba-152">JSON Representation</span></span>
<span data-ttu-id="b67ba-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b67ba-153">Here is a JSON representation of the resource.</span></span>
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




---
title: policySetItem 资源类型
description: 包含用于 PolicySet 项目的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 77438e4b0322dcb6feade0aab57c830869832e14
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287926"
---
# <a name="policysetitem-resource-type"></a><span data-ttu-id="d5479-103">policySetItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5479-103">policySetItem resource type</span></span>

<span data-ttu-id="d5479-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5479-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5479-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d5479-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5479-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5479-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5479-107">包含用于 PolicySet 项目的属性的类。</span><span class="sxs-lookup"><span data-stu-id="d5479-107">A class containing the properties used for PolicySet Item.</span></span>

## <a name="methods"></a><span data-ttu-id="d5479-108">Methods</span><span class="sxs-lookup"><span data-stu-id="d5479-108">Methods</span></span>
|<span data-ttu-id="d5479-109">方法</span><span class="sxs-lookup"><span data-stu-id="d5479-109">Method</span></span>|<span data-ttu-id="d5479-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d5479-110">Return Type</span></span>|<span data-ttu-id="d5479-111">Description</span><span class="sxs-lookup"><span data-stu-id="d5479-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d5479-112">列出 policySetItems</span><span class="sxs-lookup"><span data-stu-id="d5479-112">List policySetItems</span></span>](../api/intune-policyset-policysetitem-list.md)|<span data-ttu-id="d5479-113">[policySetItem](../resources/intune-policyset-policysetitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5479-113">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="d5479-114">列出 [policySetItem](../resources/intune-policyset-policysetitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d5479-114">List properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) objects.</span></span>|
|[<span data-ttu-id="d5479-115">获取 policySetItem</span><span class="sxs-lookup"><span data-stu-id="d5479-115">Get policySetItem</span></span>](../api/intune-policyset-policysetitem-get.md)|[<span data-ttu-id="d5479-116">policySetItem</span><span class="sxs-lookup"><span data-stu-id="d5479-116">policySetItem</span></span>](../resources/intune-policyset-policysetitem.md)|<span data-ttu-id="d5479-117">读取 [policySetItem](../resources/intune-policyset-policysetitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d5479-117">Read properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5479-118">属性</span><span class="sxs-lookup"><span data-stu-id="d5479-118">Properties</span></span>
|<span data-ttu-id="d5479-119">属性</span><span class="sxs-lookup"><span data-stu-id="d5479-119">Property</span></span>|<span data-ttu-id="d5479-120">类型</span><span class="sxs-lookup"><span data-stu-id="d5479-120">Type</span></span>|<span data-ttu-id="d5479-121">说明</span><span class="sxs-lookup"><span data-stu-id="d5479-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5479-122">id</span><span class="sxs-lookup"><span data-stu-id="d5479-122">id</span></span>|<span data-ttu-id="d5479-123">字符串</span><span class="sxs-lookup"><span data-stu-id="d5479-123">String</span></span>|<span data-ttu-id="d5479-124">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="d5479-124">Key of the MobileAppPolicySetItem.</span></span>|
|<span data-ttu-id="d5479-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5479-125">createdDateTime</span></span>|<span data-ttu-id="d5479-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5479-126">DateTimeOffset</span></span>|<span data-ttu-id="d5479-127">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="d5479-127">Creation time of the PolicySetItem.</span></span>|
|<span data-ttu-id="d5479-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5479-128">lastModifiedDateTime</span></span>|<span data-ttu-id="d5479-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5479-129">DateTimeOffset</span></span>|<span data-ttu-id="d5479-130">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="d5479-130">Last modified time of the PolicySetItem.</span></span>|
|<span data-ttu-id="d5479-131">payloadId</span><span class="sxs-lookup"><span data-stu-id="d5479-131">payloadId</span></span>|<span data-ttu-id="d5479-132">字符串</span><span class="sxs-lookup"><span data-stu-id="d5479-132">String</span></span>|<span data-ttu-id="d5479-133">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="d5479-133">PayloadId of the PolicySetItem.</span></span>|
|<span data-ttu-id="d5479-134">itemType</span><span class="sxs-lookup"><span data-stu-id="d5479-134">itemType</span></span>|<span data-ttu-id="d5479-135">字符串</span><span class="sxs-lookup"><span data-stu-id="d5479-135">String</span></span>|<span data-ttu-id="d5479-136">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="d5479-136">policySetType of the PolicySetItem.</span></span>|
|<span data-ttu-id="d5479-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d5479-137">displayName</span></span>|<span data-ttu-id="d5479-138">字符串</span><span class="sxs-lookup"><span data-stu-id="d5479-138">String</span></span>|<span data-ttu-id="d5479-139">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="d5479-139">DisplayName of the PolicySetItem.</span></span>|
|<span data-ttu-id="d5479-140">status</span><span class="sxs-lookup"><span data-stu-id="d5479-140">status</span></span>|[<span data-ttu-id="d5479-141">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="d5479-141">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="d5479-142">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="d5479-142">Status of the PolicySetItem.</span></span> <span data-ttu-id="d5479-143">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="d5479-143">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="d5479-144">errorCode</span><span class="sxs-lookup"><span data-stu-id="d5479-144">errorCode</span></span>|[<span data-ttu-id="d5479-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="d5479-145">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="d5479-146">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="d5479-146">Error code if any occured.</span></span> <span data-ttu-id="d5479-147">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="d5479-147">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="d5479-148">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="d5479-148">guidedDeploymentTags</span></span>|<span data-ttu-id="d5479-149">String 集合</span><span class="sxs-lookup"><span data-stu-id="d5479-149">String collection</span></span>|<span data-ttu-id="d5479-150">引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="d5479-150">Tags of the guided deployment</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5479-151">关系</span><span class="sxs-lookup"><span data-stu-id="d5479-151">Relationships</span></span>
<span data-ttu-id="d5479-152">无</span><span class="sxs-lookup"><span data-stu-id="d5479-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5479-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5479-153">JSON Representation</span></span>
<span data-ttu-id="d5479-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5479-154">Here is a JSON representation of the resource.</span></span>
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





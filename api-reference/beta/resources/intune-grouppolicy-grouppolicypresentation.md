---
title: groupPolicyPresentation 资源类型
description: 组策略定义中任何其他选项的显示演示文稿的基本实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8a1e4a615999a899712ad82d2177fbb862328c2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941126"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="9b1e4-103">groupPolicyPresentation 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b1e4-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="9b1e4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b1e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b1e4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b1e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b1e4-106">组策略定义中任何其他选项的显示演示文稿的基本实体。</span><span class="sxs-lookup"><span data-stu-id="9b1e4-106">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="9b1e4-107">方法</span><span class="sxs-lookup"><span data-stu-id="9b1e4-107">Methods</span></span>
|<span data-ttu-id="9b1e4-108">方法</span><span class="sxs-lookup"><span data-stu-id="9b1e4-108">Method</span></span>|<span data-ttu-id="9b1e4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9b1e4-109">Return Type</span></span>|<span data-ttu-id="9b1e4-110">说明</span><span class="sxs-lookup"><span data-stu-id="9b1e4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9b1e4-111">获取 groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="9b1e4-111">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="9b1e4-112">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="9b1e4-112">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="9b1e4-113">读取[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9b1e4-113">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="9b1e4-114">更新 groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="9b1e4-114">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="9b1e4-115">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="9b1e4-115">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="9b1e4-116">更新[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9b1e4-116">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9b1e4-117">属性</span><span class="sxs-lookup"><span data-stu-id="9b1e4-117">Properties</span></span>
|<span data-ttu-id="9b1e4-118">属性</span><span class="sxs-lookup"><span data-stu-id="9b1e4-118">Property</span></span>|<span data-ttu-id="9b1e4-119">类型</span><span class="sxs-lookup"><span data-stu-id="9b1e4-119">Type</span></span>|<span data-ttu-id="9b1e4-120">说明</span><span class="sxs-lookup"><span data-stu-id="9b1e4-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b1e4-121">label</span><span class="sxs-lookup"><span data-stu-id="9b1e4-121">label</span></span>|<span data-ttu-id="9b1e4-122">String</span><span class="sxs-lookup"><span data-stu-id="9b1e4-122">String</span></span>|<span data-ttu-id="9b1e4-123">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="9b1e4-123">Localized text label for any presentation entity.</span></span> <span data-ttu-id="9b1e4-124">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="9b1e4-124">The default value is empty.</span></span>|
|<span data-ttu-id="9b1e4-125">id</span><span class="sxs-lookup"><span data-stu-id="9b1e4-125">id</span></span>|<span data-ttu-id="9b1e4-126">String</span><span class="sxs-lookup"><span data-stu-id="9b1e4-126">String</span></span>|<span data-ttu-id="9b1e4-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9b1e4-127">Key of the entity.</span></span>|
|<span data-ttu-id="9b1e4-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b1e4-128">lastModifiedDateTime</span></span>|<span data-ttu-id="9b1e4-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b1e4-129">DateTimeOffset</span></span>|<span data-ttu-id="9b1e4-130">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9b1e4-130">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b1e4-131">关系</span><span class="sxs-lookup"><span data-stu-id="9b1e4-131">Relationships</span></span>
|<span data-ttu-id="9b1e4-132">关系</span><span class="sxs-lookup"><span data-stu-id="9b1e4-132">Relationship</span></span>|<span data-ttu-id="9b1e4-133">类型</span><span class="sxs-lookup"><span data-stu-id="9b1e4-133">Type</span></span>|<span data-ttu-id="9b1e4-134">说明</span><span class="sxs-lookup"><span data-stu-id="9b1e4-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b1e4-135">定义</span><span class="sxs-lookup"><span data-stu-id="9b1e4-135">definition</span></span>|[<span data-ttu-id="9b1e4-136">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9b1e4-136">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="9b1e4-137">与演示文稿相关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="9b1e4-137">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b1e4-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b1e4-138">JSON Representation</span></span>
<span data-ttu-id="9b1e4-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b1e4-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```





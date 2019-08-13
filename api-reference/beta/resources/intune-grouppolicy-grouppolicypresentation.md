---
title: groupPolicyPresentation 资源类型
description: 组策略定义中任何其他选项的显示演示文稿的基本实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ee950b7e4e292b9fb177778ff4df2dcb51641e54
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331432"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="3879c-103">groupPolicyPresentation 资源类型</span><span class="sxs-lookup"><span data-stu-id="3879c-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="3879c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3879c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3879c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3879c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3879c-106">组策略定义中任何其他选项的显示演示文稿的基本实体。</span><span class="sxs-lookup"><span data-stu-id="3879c-106">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="3879c-107">方法</span><span class="sxs-lookup"><span data-stu-id="3879c-107">Methods</span></span>
|<span data-ttu-id="3879c-108">方法</span><span class="sxs-lookup"><span data-stu-id="3879c-108">Method</span></span>|<span data-ttu-id="3879c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3879c-109">Return Type</span></span>|<span data-ttu-id="3879c-110">说明</span><span class="sxs-lookup"><span data-stu-id="3879c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3879c-111">获取 groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="3879c-111">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="3879c-112">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="3879c-112">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="3879c-113">读取[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3879c-113">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="3879c-114">更新 groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="3879c-114">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="3879c-115">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="3879c-115">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="3879c-116">更新[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3879c-116">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3879c-117">属性</span><span class="sxs-lookup"><span data-stu-id="3879c-117">Properties</span></span>
|<span data-ttu-id="3879c-118">属性</span><span class="sxs-lookup"><span data-stu-id="3879c-118">Property</span></span>|<span data-ttu-id="3879c-119">类型</span><span class="sxs-lookup"><span data-stu-id="3879c-119">Type</span></span>|<span data-ttu-id="3879c-120">说明</span><span class="sxs-lookup"><span data-stu-id="3879c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3879c-121">label</span><span class="sxs-lookup"><span data-stu-id="3879c-121">label</span></span>|<span data-ttu-id="3879c-122">String</span><span class="sxs-lookup"><span data-stu-id="3879c-122">String</span></span>|<span data-ttu-id="3879c-123">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="3879c-123">Localized text label for any presentation entity.</span></span> <span data-ttu-id="3879c-124">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="3879c-124">The default value is empty.</span></span>|
|<span data-ttu-id="3879c-125">id</span><span class="sxs-lookup"><span data-stu-id="3879c-125">id</span></span>|<span data-ttu-id="3879c-126">String</span><span class="sxs-lookup"><span data-stu-id="3879c-126">String</span></span>|<span data-ttu-id="3879c-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3879c-127">Key of the entity.</span></span>|
|<span data-ttu-id="3879c-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3879c-128">lastModifiedDateTime</span></span>|<span data-ttu-id="3879c-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3879c-129">DateTimeOffset</span></span>|<span data-ttu-id="3879c-130">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3879c-130">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3879c-131">关系</span><span class="sxs-lookup"><span data-stu-id="3879c-131">Relationships</span></span>
|<span data-ttu-id="3879c-132">关系</span><span class="sxs-lookup"><span data-stu-id="3879c-132">Relationship</span></span>|<span data-ttu-id="3879c-133">类型</span><span class="sxs-lookup"><span data-stu-id="3879c-133">Type</span></span>|<span data-ttu-id="3879c-134">说明</span><span class="sxs-lookup"><span data-stu-id="3879c-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3879c-135">定义</span><span class="sxs-lookup"><span data-stu-id="3879c-135">definition</span></span>|[<span data-ttu-id="3879c-136">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="3879c-136">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="3879c-137">与演示文稿相关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="3879c-137">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3879c-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3879c-138">JSON Representation</span></span>
<span data-ttu-id="3879c-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3879c-139">Here is a JSON representation of the resource.</span></span>
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




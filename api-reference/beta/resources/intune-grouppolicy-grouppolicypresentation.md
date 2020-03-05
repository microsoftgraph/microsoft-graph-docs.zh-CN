---
title: groupPolicyPresentation 资源类型
description: 组策略定义中任何其他选项的显示演示文稿的基本实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8a829f974a25412a88dcc44ef5e9b84a0c3f81a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528081"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="780d2-103">groupPolicyPresentation 资源类型</span><span class="sxs-lookup"><span data-stu-id="780d2-103">groupPolicyPresentation resource type</span></span>

<span data-ttu-id="780d2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="780d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="780d2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="780d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="780d2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="780d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="780d2-107">组策略定义中任何其他选项的显示演示文稿的基本实体。</span><span class="sxs-lookup"><span data-stu-id="780d2-107">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="780d2-108">方法</span><span class="sxs-lookup"><span data-stu-id="780d2-108">Methods</span></span>
|<span data-ttu-id="780d2-109">方法</span><span class="sxs-lookup"><span data-stu-id="780d2-109">Method</span></span>|<span data-ttu-id="780d2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="780d2-110">Return Type</span></span>|<span data-ttu-id="780d2-111">说明</span><span class="sxs-lookup"><span data-stu-id="780d2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="780d2-112">获取 groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="780d2-112">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="780d2-113">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="780d2-113">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="780d2-114">读取[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="780d2-114">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="780d2-115">更新 groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="780d2-115">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="780d2-116">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="780d2-116">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="780d2-117">更新[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="780d2-117">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="780d2-118">属性</span><span class="sxs-lookup"><span data-stu-id="780d2-118">Properties</span></span>
|<span data-ttu-id="780d2-119">属性</span><span class="sxs-lookup"><span data-stu-id="780d2-119">Property</span></span>|<span data-ttu-id="780d2-120">类型</span><span class="sxs-lookup"><span data-stu-id="780d2-120">Type</span></span>|<span data-ttu-id="780d2-121">说明</span><span class="sxs-lookup"><span data-stu-id="780d2-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="780d2-122">label</span><span class="sxs-lookup"><span data-stu-id="780d2-122">label</span></span>|<span data-ttu-id="780d2-123">String</span><span class="sxs-lookup"><span data-stu-id="780d2-123">String</span></span>|<span data-ttu-id="780d2-124">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="780d2-124">Localized text label for any presentation entity.</span></span> <span data-ttu-id="780d2-125">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="780d2-125">The default value is empty.</span></span>|
|<span data-ttu-id="780d2-126">id</span><span class="sxs-lookup"><span data-stu-id="780d2-126">id</span></span>|<span data-ttu-id="780d2-127">String</span><span class="sxs-lookup"><span data-stu-id="780d2-127">String</span></span>|<span data-ttu-id="780d2-128">实体的键。</span><span class="sxs-lookup"><span data-stu-id="780d2-128">Key of the entity.</span></span>|
|<span data-ttu-id="780d2-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="780d2-129">lastModifiedDateTime</span></span>|<span data-ttu-id="780d2-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="780d2-130">DateTimeOffset</span></span>|<span data-ttu-id="780d2-131">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="780d2-131">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="780d2-132">关系</span><span class="sxs-lookup"><span data-stu-id="780d2-132">Relationships</span></span>
|<span data-ttu-id="780d2-133">关系</span><span class="sxs-lookup"><span data-stu-id="780d2-133">Relationship</span></span>|<span data-ttu-id="780d2-134">类型</span><span class="sxs-lookup"><span data-stu-id="780d2-134">Type</span></span>|<span data-ttu-id="780d2-135">说明</span><span class="sxs-lookup"><span data-stu-id="780d2-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="780d2-136">定义</span><span class="sxs-lookup"><span data-stu-id="780d2-136">definition</span></span>|[<span data-ttu-id="780d2-137">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="780d2-137">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="780d2-138">与演示文稿相关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="780d2-138">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="780d2-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="780d2-139">JSON Representation</span></span>
<span data-ttu-id="780d2-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="780d2-140">Here is a JSON representation of the resource.</span></span>
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




---
title: groupPolicyPresentation 资源类型
description: 显示演示文稿中的组策略定义的其他选项的任何基准实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 736b599eaf310bc63530daa45ffa1aee7ede4c3f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429571"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="cf5c6-103">groupPolicyPresentation 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf5c6-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="cf5c6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="cf5c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cf5c6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cf5c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf5c6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cf5c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf5c6-107">显示演示文稿中的组策略定义的其他选项的任何基准实体。</span><span class="sxs-lookup"><span data-stu-id="cf5c6-107">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="cf5c6-108">方法</span><span class="sxs-lookup"><span data-stu-id="cf5c6-108">Methods</span></span>
|<span data-ttu-id="cf5c6-109">方法</span><span class="sxs-lookup"><span data-stu-id="cf5c6-109">Method</span></span>|<span data-ttu-id="cf5c6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cf5c6-110">Return Type</span></span>|<span data-ttu-id="cf5c6-111">说明</span><span class="sxs-lookup"><span data-stu-id="cf5c6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cf5c6-112">获取 groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="cf5c6-112">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="cf5c6-113">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="cf5c6-113">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="cf5c6-114">读取属性和[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="cf5c6-114">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="cf5c6-115">更新 groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="cf5c6-115">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="cf5c6-116">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="cf5c6-116">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="cf5c6-117">更新[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cf5c6-117">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cf5c6-118">属性</span><span class="sxs-lookup"><span data-stu-id="cf5c6-118">Properties</span></span>
|<span data-ttu-id="cf5c6-119">属性</span><span class="sxs-lookup"><span data-stu-id="cf5c6-119">Property</span></span>|<span data-ttu-id="cf5c6-120">类型</span><span class="sxs-lookup"><span data-stu-id="cf5c6-120">Type</span></span>|<span data-ttu-id="cf5c6-121">说明</span><span class="sxs-lookup"><span data-stu-id="cf5c6-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf5c6-122">标签</span><span class="sxs-lookup"><span data-stu-id="cf5c6-122">label</span></span>|<span data-ttu-id="cf5c6-123">String</span><span class="sxs-lookup"><span data-stu-id="cf5c6-123">String</span></span>|<span data-ttu-id="cf5c6-124">任何演示文稿实体的本地化的文本标签。</span><span class="sxs-lookup"><span data-stu-id="cf5c6-124">Localized text label for any presentation entity.</span></span> <span data-ttu-id="cf5c6-125">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="cf5c6-125">The default value is empty.</span></span>|
|<span data-ttu-id="cf5c6-126">id</span><span class="sxs-lookup"><span data-stu-id="cf5c6-126">id</span></span>|<span data-ttu-id="cf5c6-127">String</span><span class="sxs-lookup"><span data-stu-id="cf5c6-127">String</span></span>|<span data-ttu-id="cf5c6-128">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cf5c6-128">Key of the entity.</span></span>|
|<span data-ttu-id="cf5c6-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf5c6-129">lastModifiedDateTime</span></span>|<span data-ttu-id="cf5c6-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf5c6-130">DateTimeOffset</span></span>|<span data-ttu-id="cf5c6-131">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="cf5c6-131">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf5c6-132">关系</span><span class="sxs-lookup"><span data-stu-id="cf5c6-132">Relationships</span></span>
|<span data-ttu-id="cf5c6-133">关系</span><span class="sxs-lookup"><span data-stu-id="cf5c6-133">Relationship</span></span>|<span data-ttu-id="cf5c6-134">类型</span><span class="sxs-lookup"><span data-stu-id="cf5c6-134">Type</span></span>|<span data-ttu-id="cf5c6-135">说明</span><span class="sxs-lookup"><span data-stu-id="cf5c6-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf5c6-136">definition</span><span class="sxs-lookup"><span data-stu-id="cf5c6-136">definition</span></span>|[<span data-ttu-id="cf5c6-137">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="cf5c6-137">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="cf5c6-138">随演示文稿相关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="cf5c6-138">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf5c6-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf5c6-139">JSON Representation</span></span>
<span data-ttu-id="cf5c6-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf5c6-140">Here is a JSON representation of the resource.</span></span>
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





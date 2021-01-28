---
title: educationAssignmentSettings 资源类型
description: 指定课堂级别作业设置。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c670cb2bbef0b82ff80996e4acb52c2826ec118f
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034333"
---
# <a name="educationassignmentsettings-resource-type"></a><span data-ttu-id="84e6f-103">educationAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="84e6f-103">educationAssignmentSettings resource type</span></span>

<span data-ttu-id="84e6f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84e6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84e6f-105">指定课堂级别作业设置。</span><span class="sxs-lookup"><span data-stu-id="84e6f-105">Specifies class-level assignments settings.</span></span>

## <a name="methods"></a><span data-ttu-id="84e6f-106">方法</span><span class="sxs-lookup"><span data-stu-id="84e6f-106">Methods</span></span>
|<span data-ttu-id="84e6f-107">方法</span><span class="sxs-lookup"><span data-stu-id="84e6f-107">Method</span></span>|<span data-ttu-id="84e6f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="84e6f-108">Return type</span></span>|<span data-ttu-id="84e6f-109">说明</span><span class="sxs-lookup"><span data-stu-id="84e6f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84e6f-110">获取 educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="84e6f-110">Get educationAssignmentSettings</span></span>](../api/educationassignmentsettings-get.md)|[<span data-ttu-id="84e6f-111">educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="84e6f-111">educationAssignmentSettings</span></span>](../resources/educationassignmentsettings.md)|<span data-ttu-id="84e6f-112">读取 [educationAssignmentSettings 对象的属性和](../resources/educationassignmentsettings.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="84e6f-112">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>|
|[<span data-ttu-id="84e6f-113">更新 educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="84e6f-113">Update educationAssignmentSettings</span></span>](../api/educationassignmentsettings-update.md)|[<span data-ttu-id="84e6f-114">educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="84e6f-114">educationAssignmentSettings</span></span>](../resources/educationassignmentsettings.md)|<span data-ttu-id="84e6f-115">更新 [educationAssignmentSettings 对象](../resources/educationassignmentsettings.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="84e6f-115">Update the properties of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="84e6f-116">属性</span><span class="sxs-lookup"><span data-stu-id="84e6f-116">Properties</span></span>
|<span data-ttu-id="84e6f-117">属性</span><span class="sxs-lookup"><span data-stu-id="84e6f-117">Property</span></span>|<span data-ttu-id="84e6f-118">类型</span><span class="sxs-lookup"><span data-stu-id="84e6f-118">Type</span></span>|<span data-ttu-id="84e6f-119">说明</span><span class="sxs-lookup"><span data-stu-id="84e6f-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84e6f-120">submissionAnimationDisabled</span><span class="sxs-lookup"><span data-stu-id="84e6f-120">submissionAnimationDisabled</span></span>|<span data-ttu-id="84e6f-121">布尔</span><span class="sxs-lookup"><span data-stu-id="84e6f-121">Boolean</span></span>|<span data-ttu-id="84e6f-122">指示是否显示打开的庆祝动画。</span><span class="sxs-lookup"><span data-stu-id="84e6f-122">Indicates whether turn-in celebration animation will be shown.</span></span> <span data-ttu-id="84e6f-123">值 `true` 指示不会显示动画。</span><span class="sxs-lookup"><span data-stu-id="84e6f-123">A value of `true` indicates that the animation will not be shown.</span></span> <span data-ttu-id="84e6f-124">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="84e6f-124">Default value is `false`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84e6f-125">关系</span><span class="sxs-lookup"><span data-stu-id="84e6f-125">Relationships</span></span>
<span data-ttu-id="84e6f-126">无。</span><span class="sxs-lookup"><span data-stu-id="84e6f-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="84e6f-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84e6f-127">JSON representation</span></span>
<span data-ttu-id="84e6f-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84e6f-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentSettings",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "submissionAnimationDisabled": false
}
```


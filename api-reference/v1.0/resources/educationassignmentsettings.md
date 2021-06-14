---
title: educationAssignmentSettings 资源类型
description: 指定课堂级别的作业设置。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ccaa51c84e50e2f9c5302836ffd9b92754f517fd
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912353"
---
# <a name="educationassignmentsettings-resource-type"></a><span data-ttu-id="53198-103">educationAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="53198-103">educationAssignmentSettings resource type</span></span>

<span data-ttu-id="53198-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53198-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53198-105">指定课堂级别的作业设置。</span><span class="sxs-lookup"><span data-stu-id="53198-105">Specifies class-level assignments settings.</span></span>

## <a name="methods"></a><span data-ttu-id="53198-106">方法</span><span class="sxs-lookup"><span data-stu-id="53198-106">Methods</span></span>
|<span data-ttu-id="53198-107">方法</span><span class="sxs-lookup"><span data-stu-id="53198-107">Method</span></span>|<span data-ttu-id="53198-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="53198-108">Return type</span></span>|<span data-ttu-id="53198-109">说明</span><span class="sxs-lookup"><span data-stu-id="53198-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="53198-110">获取 educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="53198-110">Get educationAssignmentSettings</span></span>](../api/educationassignmentsettings-get.md)|[<span data-ttu-id="53198-111">educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="53198-111">educationAssignmentSettings</span></span>](../resources/educationassignmentsettings.md)|<span data-ttu-id="53198-112">读取 [educationAssignmentSettings 对象的属性和](../resources/educationassignmentsettings.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="53198-112">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>|
|[<span data-ttu-id="53198-113">更新 educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="53198-113">Update educationAssignmentSettings</span></span>](../api/educationassignmentsettings-update.md)|[<span data-ttu-id="53198-114">educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="53198-114">educationAssignmentSettings</span></span>](../resources/educationassignmentsettings.md)|<span data-ttu-id="53198-115">更新 [educationAssignmentSettings 对象](../resources/educationassignmentsettings.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="53198-115">Update the properties of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="53198-116">属性</span><span class="sxs-lookup"><span data-stu-id="53198-116">Properties</span></span>
|<span data-ttu-id="53198-117">属性</span><span class="sxs-lookup"><span data-stu-id="53198-117">Property</span></span>|<span data-ttu-id="53198-118">类型</span><span class="sxs-lookup"><span data-stu-id="53198-118">Type</span></span>|<span data-ttu-id="53198-119">说明</span><span class="sxs-lookup"><span data-stu-id="53198-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53198-120">submissionAnimationDisabled</span><span class="sxs-lookup"><span data-stu-id="53198-120">submissionAnimationDisabled</span></span>|<span data-ttu-id="53198-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="53198-121">Boolean</span></span>|<span data-ttu-id="53198-122">指示是否显示打开的庆祝动画。</span><span class="sxs-lookup"><span data-stu-id="53198-122">Indicates whether turn-in celebration animation will be shown.</span></span> <span data-ttu-id="53198-123">的值 `true` 指示不会显示动画。</span><span class="sxs-lookup"><span data-stu-id="53198-123">A value of `true` indicates that the animation will not be shown.</span></span> <span data-ttu-id="53198-124">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="53198-124">Default value is `false`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53198-125">关系</span><span class="sxs-lookup"><span data-stu-id="53198-125">Relationships</span></span>
<span data-ttu-id="53198-126">无。</span><span class="sxs-lookup"><span data-stu-id="53198-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="53198-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53198-127">JSON representation</span></span>
<span data-ttu-id="53198-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53198-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentSettings",
  "openType": false
}
-->
``` json
{
  "submissionAnimationDisabled": false
}
```


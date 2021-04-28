---
title: qualityUpdateReference 资源类型
description: 表示Windows 10更新内容。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ca416ba5031e4642a073f4796ee27996d22f0f5a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067852"
---
# <a name="qualityupdatereference-resource-type"></a><span data-ttu-id="66069-103">qualityUpdateReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="66069-103">qualityUpdateReference resource type</span></span>

<span data-ttu-id="66069-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="66069-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66069-105">表示Windows 10更新内容。</span><span class="sxs-lookup"><span data-stu-id="66069-105">Represents Windows 10 quality update content.</span></span>

<span data-ttu-id="66069-106">在部署中，相同的质量更新参考可能会导致设备接收不同的更新修订，但内容被视为与部署中所有设备的上下文等效。</span><span class="sxs-lookup"><span data-stu-id="66069-106">In a deployment, the same quality update reference could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="66069-107">继承自 [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md)。</span><span class="sxs-lookup"><span data-stu-id="66069-107">Inherits from [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span></span> <span data-ttu-id="66069-108">[expeditedQualityUpdateReference 的基本类型](../resources/windowsupdates-expeditedqualityupdatereference.md)。</span><span class="sxs-lookup"><span data-stu-id="66069-108">Base type of [expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).</span></span>

## <a name="properties"></a><span data-ttu-id="66069-109">属性</span><span class="sxs-lookup"><span data-stu-id="66069-109">Properties</span></span>
|<span data-ttu-id="66069-110">属性</span><span class="sxs-lookup"><span data-stu-id="66069-110">Property</span></span>|<span data-ttu-id="66069-111">类型</span><span class="sxs-lookup"><span data-stu-id="66069-111">Type</span></span>|<span data-ttu-id="66069-112">说明</span><span class="sxs-lookup"><span data-stu-id="66069-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66069-113">classification</span><span class="sxs-lookup"><span data-stu-id="66069-113">classification</span></span>|<span data-ttu-id="66069-114">microsoft.graph.windowsUpdates.qualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="66069-114">microsoft.graph.windowsUpdates.qualityUpdateClassification</span></span>|<span data-ttu-id="66069-115">指定所引用内容的分类。</span><span class="sxs-lookup"><span data-stu-id="66069-115">Specifies the classification of the referenced content.</span></span> <span data-ttu-id="66069-116">支持 **qualityUpdateClassification 值的子集**。</span><span class="sxs-lookup"><span data-stu-id="66069-116">Supports a subset of the values for **qualityUpdateClassification**.</span></span> <span data-ttu-id="66069-117">可能的值是 `security` ：。</span><span class="sxs-lookup"><span data-stu-id="66069-117">Possible values are: `security`.</span></span>|
|<span data-ttu-id="66069-118">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="66069-118">releaseDateTime</span></span>|<span data-ttu-id="66069-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66069-119">DateTimeOffset</span></span>|<span data-ttu-id="66069-120">指定给定 servicingChannel 中的质量更新，按日期 (给定分类，即指定日期发布) 。</span><span class="sxs-lookup"><span data-stu-id="66069-120">Specifies a quality update in the given servicingChannel with the given classification by date (i.e. the last update published on the specified date).</span></span> <span data-ttu-id="66069-121">默认值为 security。</span><span class="sxs-lookup"><span data-stu-id="66069-121">Default value is security.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66069-122">关系</span><span class="sxs-lookup"><span data-stu-id="66069-122">Relationships</span></span>
<span data-ttu-id="66069-123">无。</span><span class="sxs-lookup"><span data-stu-id="66069-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66069-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66069-124">JSON representation</span></span>
<span data-ttu-id="66069-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66069-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.qualityUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateReference",
  "classification": "String",
  "releaseDateTime": "String (timestamp)"
}
```


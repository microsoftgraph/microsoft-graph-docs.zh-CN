---
title: featureUpdateReference 资源类型
description: 表示Windows 10更新内容。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 69eda05a94982429035999bd914c6f0c9847fa67
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067331"
---
# <a name="featureupdatereference-resource-type"></a><span data-ttu-id="4b920-103">featureUpdateReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b920-103">featureUpdateReference resource type</span></span>

<span data-ttu-id="4b920-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="4b920-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b920-105">表示Windows 10更新内容。</span><span class="sxs-lookup"><span data-stu-id="4b920-105">Represents Windows 10 feature update content.</span></span>

<span data-ttu-id="4b920-106">在部署中，相同的功能更新引用可能会导致设备接收不同的更新修订，但内容被视为与部署中所有设备的上下文等效。</span><span class="sxs-lookup"><span data-stu-id="4b920-106">In a deployment, the same feature update reference could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="4b920-107">继承自 [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md)。</span><span class="sxs-lookup"><span data-stu-id="4b920-107">Inherits from [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4b920-108">属性</span><span class="sxs-lookup"><span data-stu-id="4b920-108">Properties</span></span>
|<span data-ttu-id="4b920-109">属性</span><span class="sxs-lookup"><span data-stu-id="4b920-109">Property</span></span>|<span data-ttu-id="4b920-110">类型</span><span class="sxs-lookup"><span data-stu-id="4b920-110">Type</span></span>|<span data-ttu-id="4b920-111">说明</span><span class="sxs-lookup"><span data-stu-id="4b920-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b920-112">version</span><span class="sxs-lookup"><span data-stu-id="4b920-112">version</span></span>|<span data-ttu-id="4b920-113">String</span><span class="sxs-lookup"><span data-stu-id="4b920-113">String</span></span>|<span data-ttu-id="4b920-114">按版本指定功能更新。</span><span class="sxs-lookup"><span data-stu-id="4b920-114">Specifies a feature update by version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b920-115">关系</span><span class="sxs-lookup"><span data-stu-id="4b920-115">Relationships</span></span>
<span data-ttu-id="4b920-116">无。</span><span class="sxs-lookup"><span data-stu-id="4b920-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b920-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b920-117">JSON representation</span></span>
<span data-ttu-id="4b920-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b920-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateReference",
  "version": "String"
}
```


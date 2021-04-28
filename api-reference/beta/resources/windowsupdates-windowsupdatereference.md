---
title: windowsUpdateReference 资源类型
description: 表示特定Windows 10内容。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a75f1afe1c2689760848283bf078b957bb8739ba
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067256"
---
# <a name="windowsupdatereference-resource-type"></a><span data-ttu-id="6c531-103">windowsUpdateReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c531-103">windowsUpdateReference resource type</span></span>

<span data-ttu-id="6c531-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="6c531-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c531-105">表示特定Windows 10内容。</span><span class="sxs-lookup"><span data-stu-id="6c531-105">Represents specific Windows 10 update content.</span></span>

<span data-ttu-id="6c531-106">在部署中，相同的Windows引用可能会导致设备接收不同的更新修订，但内容被视为与部署中所有设备的上下文等效。</span><span class="sxs-lookup"><span data-stu-id="6c531-106">In a deployment, the same Windows update reference could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="6c531-107">所有Windows引用作为以下派生类型之一存在[：featureUpdateReference](../resources/windowsupdates-featureupdatereference.md)和[expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md)。</span><span class="sxs-lookup"><span data-stu-id="6c531-107">All Windows update references exist as one of the following derived types: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) and [expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).</span></span>

<span data-ttu-id="6c531-108">继承自 [softwareUpdateReference](../resources/windowsupdates-softwareupdatereference.md)。</span><span class="sxs-lookup"><span data-stu-id="6c531-108">Inherits from [softwareUpdateReference](../resources/windowsupdates-softwareupdatereference.md).</span></span> <span data-ttu-id="6c531-109">[featureUpdateReference](../resources/windowsupdates-featureupdatereference.md)和[qualityUpdateReference 的基类型](../resources/windowsupdates-qualityupdatereference.md)。</span><span class="sxs-lookup"><span data-stu-id="6c531-109">Base type for [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) and [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span></span>

<span data-ttu-id="6c531-110">这是一个抽象类型。</span><span class="sxs-lookup"><span data-stu-id="6c531-110">This is an abstract type.</span></span>

## <a name="properties"></a><span data-ttu-id="6c531-111">属性</span><span class="sxs-lookup"><span data-stu-id="6c531-111">Properties</span></span>
<span data-ttu-id="6c531-112">无。</span><span class="sxs-lookup"><span data-stu-id="6c531-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="6c531-113">关系</span><span class="sxs-lookup"><span data-stu-id="6c531-113">Relationships</span></span>
<span data-ttu-id="6c531-114">无。</span><span class="sxs-lookup"><span data-stu-id="6c531-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c531-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c531-115">JSON representation</span></span>
<span data-ttu-id="6c531-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c531-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.windowsUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windowsUpdateReference"
}
```


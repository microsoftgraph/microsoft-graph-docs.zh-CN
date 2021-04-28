---
title: softwareUpdateReference 资源类型
description: 表示特定更新内容。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 66f7f895bd3d7556ad5e3d35066236663b474f41
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067973"
---
# <a name="softwareupdatereference-resource-type"></a><span data-ttu-id="383c0-103">softwareUpdateReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="383c0-103">softwareUpdateReference resource type</span></span>

<span data-ttu-id="383c0-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="383c0-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="383c0-105">表示特定更新内容。</span><span class="sxs-lookup"><span data-stu-id="383c0-105">Represents specific update content.</span></span>

<span data-ttu-id="383c0-106">在部署中，相同的 **softwareUpdateReference** 可能会导致设备接收不同的更新修订，但内容被视为与部署中所有设备的上下文等效。</span><span class="sxs-lookup"><span data-stu-id="383c0-106">In a deployment, the same **softwareUpdateReference** could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="383c0-107">所有软件更新引用作为以下派生类型之一存在 [：featureUpdateReference](../resources/windowsupdates-featureupdatereference.md)。</span><span class="sxs-lookup"><span data-stu-id="383c0-107">All software update references exist as one of the following derived types: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md).</span></span>

<span data-ttu-id="383c0-108">继承自 [deployableContent](../resources/windowsupdates-deployablecontent.md)。</span><span class="sxs-lookup"><span data-stu-id="383c0-108">Inherits from [deployableContent](../resources/windowsupdates-deployablecontent.md).</span></span> <span data-ttu-id="383c0-109">[windowsUpdateReference 的基类型](../resources/windowsupdates-windowsupdatereference.md)。</span><span class="sxs-lookup"><span data-stu-id="383c0-109">Base type for [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span></span>

<span data-ttu-id="383c0-110">这是一个抽象类型。</span><span class="sxs-lookup"><span data-stu-id="383c0-110">This is an abstract type.</span></span>

## <a name="properties"></a><span data-ttu-id="383c0-111">属性</span><span class="sxs-lookup"><span data-stu-id="383c0-111">Properties</span></span>
<span data-ttu-id="383c0-112">无。</span><span class="sxs-lookup"><span data-stu-id="383c0-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="383c0-113">关系</span><span class="sxs-lookup"><span data-stu-id="383c0-113">Relationships</span></span>
<span data-ttu-id="383c0-114">无。</span><span class="sxs-lookup"><span data-stu-id="383c0-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="383c0-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="383c0-115">JSON representation</span></span>
<span data-ttu-id="383c0-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="383c0-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.softwareUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.softwareUpdateReference"
}
```


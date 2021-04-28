---
title: windows 资源类型
description: 充当功能容器Windows实体。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3f7677f97db8d57e1fba74174df8cd848ad4f224
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067295"
---
# <a name="windows-resource-type"></a><span data-ttu-id="854e0-103">windows 资源类型</span><span class="sxs-lookup"><span data-stu-id="854e0-103">windows resource type</span></span>

<span data-ttu-id="854e0-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="854e0-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="854e0-105">充当功能容器Windows实体。</span><span class="sxs-lookup"><span data-stu-id="854e0-105">Entity that acts as a container for Windows functionality.</span></span>

## <a name="properties"></a><span data-ttu-id="854e0-106">属性</span><span class="sxs-lookup"><span data-stu-id="854e0-106">Properties</span></span>
|<span data-ttu-id="854e0-107">属性</span><span class="sxs-lookup"><span data-stu-id="854e0-107">Property</span></span>|<span data-ttu-id="854e0-108">类型</span><span class="sxs-lookup"><span data-stu-id="854e0-108">Type</span></span>|<span data-ttu-id="854e0-109">说明</span><span class="sxs-lookup"><span data-stu-id="854e0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="854e0-110">id</span><span class="sxs-lookup"><span data-stu-id="854e0-110">id</span></span>|<span data-ttu-id="854e0-111">String</span><span class="sxs-lookup"><span data-stu-id="854e0-111">String</span></span>|<span data-ttu-id="854e0-112">只读。</span><span class="sxs-lookup"><span data-stu-id="854e0-112">Read-only.</span></span> <span data-ttu-id="854e0-113">继承自 [实体](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="854e0-113">Inherited from [entity](../resources/entity.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="854e0-114">关系</span><span class="sxs-lookup"><span data-stu-id="854e0-114">Relationships</span></span>
|<span data-ttu-id="854e0-115">关系</span><span class="sxs-lookup"><span data-stu-id="854e0-115">Relationship</span></span>|<span data-ttu-id="854e0-116">类型</span><span class="sxs-lookup"><span data-stu-id="854e0-116">Type</span></span>|<span data-ttu-id="854e0-117">说明</span><span class="sxs-lookup"><span data-stu-id="854e0-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="854e0-118">updates</span><span class="sxs-lookup"><span data-stu-id="854e0-118">updates</span></span>|[<span data-ttu-id="854e0-119">microsoft.graph.windowsUpdates.updates</span><span class="sxs-lookup"><span data-stu-id="854e0-119">microsoft.graph.windowsUpdates.updates</span></span>](../resources/windowsupdates-updates.md)|<span data-ttu-id="854e0-120">充当 Windows Update for Business 部署服务功能的容器的实体。</span><span class="sxs-lookup"><span data-stu-id="854e0-120">Entity that acts as a container for the functionality of the Windows Update for Business deployment service.</span></span> <span data-ttu-id="854e0-121">只读。</span><span class="sxs-lookup"><span data-stu-id="854e0-121">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="854e0-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="854e0-122">JSON representation</span></span>
<span data-ttu-id="854e0-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="854e0-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.windows",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windows",
  "id": "String (identifier)"
}
```


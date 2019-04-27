---
title: changeTrackedEntity 资源类型
description: ''
localization_priority: Normal
ms.openlocfilehash: 838aeca84b6928c709a3c4775c95ab3ef8fd7692
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33347938"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="5e700-102">changeTrackedEntity 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e700-102">changeTrackedEntity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="5e700-103">属性</span><span class="sxs-lookup"><span data-stu-id="5e700-103">Properties</span></span>
|<span data-ttu-id="5e700-104">属性</span><span class="sxs-lookup"><span data-stu-id="5e700-104">Property</span></span>|<span data-ttu-id="5e700-105">类型</span><span class="sxs-lookup"><span data-stu-id="5e700-105">Type</span></span>|<span data-ttu-id="5e700-106">说明</span><span class="sxs-lookup"><span data-stu-id="5e700-106">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e700-107">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e700-107">createdDateTime</span></span>| <span data-ttu-id="5e700-108">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e700-108">DateTimeOffset</span></span>| |
|<span data-ttu-id="5e700-109">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e700-109">lastModifiedDateTime</span></span>| <span data-ttu-id="5e700-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e700-110">DateTimeOffset</span></span>| |
|<span data-ttu-id="5e700-111">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5e700-111">lastModifiedBy</span></span>| [<span data-ttu-id="5e700-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="5e700-112">identitySet</span></span>](identityset.md) | |

## <a name="relationships"></a><span data-ttu-id="5e700-113">关系</span><span class="sxs-lookup"><span data-stu-id="5e700-113">Relationships</span></span>
<span data-ttu-id="5e700-114">无</span><span class="sxs-lookup"><span data-stu-id="5e700-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5e700-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e700-115">JSON Representation</span></span>
<span data-ttu-id="5e700-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e700-116">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.changeTrackedEntity",
  "baseType":"microsoft.graph.entity",
  "abstract":true
}-->

``` json
{
    "createdDateTime":"String (timestamp)",
    "lastModifiedDateTime" :"String (timestamp)",
    "lastModifiedBy":{"@odata.type":"microsoft.graph.identitySet"}
}
```




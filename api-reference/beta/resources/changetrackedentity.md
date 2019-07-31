---
title: changeTrackedEntity 资源类型
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3815b22c7bd76a894df0e98415e0c30bb77decd1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974051"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="711df-102">changeTrackedEntity 资源类型</span><span class="sxs-lookup"><span data-stu-id="711df-102">changeTrackedEntity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="711df-103">属性</span><span class="sxs-lookup"><span data-stu-id="711df-103">Properties</span></span>
|<span data-ttu-id="711df-104">属性</span><span class="sxs-lookup"><span data-stu-id="711df-104">Property</span></span>|<span data-ttu-id="711df-105">类型</span><span class="sxs-lookup"><span data-stu-id="711df-105">Type</span></span>|<span data-ttu-id="711df-106">说明</span><span class="sxs-lookup"><span data-stu-id="711df-106">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="711df-107">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="711df-107">createdDateTime</span></span>| <span data-ttu-id="711df-108">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="711df-108">DateTimeOffset</span></span>| |
|<span data-ttu-id="711df-109">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="711df-109">lastModifiedDateTime</span></span>| <span data-ttu-id="711df-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="711df-110">DateTimeOffset</span></span>| |
|<span data-ttu-id="711df-111">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="711df-111">lastModifiedBy</span></span>| [<span data-ttu-id="711df-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="711df-112">identitySet</span></span>](identityset.md) | |

## <a name="relationships"></a><span data-ttu-id="711df-113">关系</span><span class="sxs-lookup"><span data-stu-id="711df-113">Relationships</span></span>
<span data-ttu-id="711df-114">无</span><span class="sxs-lookup"><span data-stu-id="711df-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="711df-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="711df-115">JSON Representation</span></span>
<span data-ttu-id="711df-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="711df-116">Here is a JSON representation of the resource.</span></span>
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




---
title: accessPackageLocalizedText 资源类型
description: 用于表示特定语言中的字符串的复杂类型。
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8d493f0909617dcda26546ccc262d7591c6b9309
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137345"
---
# <a name="accesspackagelocalizedtext-resource-type"></a><span data-ttu-id="fcda9-103">accessPackageLocalizedText 资源类型</span><span class="sxs-lookup"><span data-stu-id="fcda9-103">accessPackageLocalizedText resource type</span></span>

<span data-ttu-id="fcda9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcda9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcda9-105">用于表示特定语言中的字符串的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="fcda9-105">A complex type used to represent a string in a specific language.</span></span>

## <a name="properties"></a><span data-ttu-id="fcda9-106">属性</span><span class="sxs-lookup"><span data-stu-id="fcda9-106">Properties</span></span>
|<span data-ttu-id="fcda9-107">属性</span><span class="sxs-lookup"><span data-stu-id="fcda9-107">Property</span></span>|<span data-ttu-id="fcda9-108">类型</span><span class="sxs-lookup"><span data-stu-id="fcda9-108">Type</span></span>|<span data-ttu-id="fcda9-109">说明</span><span class="sxs-lookup"><span data-stu-id="fcda9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcda9-110">languageCode</span><span class="sxs-lookup"><span data-stu-id="fcda9-110">languageCode</span></span>|<span data-ttu-id="fcda9-111">字符串</span><span class="sxs-lookup"><span data-stu-id="fcda9-111">String</span></span>|<span data-ttu-id="fcda9-112">目标语言的 ISO 代码。</span><span class="sxs-lookup"><span data-stu-id="fcda9-112">The ISO code for the intended language.</span></span> <span data-ttu-id="fcda9-113">必填。</span><span class="sxs-lookup"><span data-stu-id="fcda9-113">Required.</span></span> |
|<span data-ttu-id="fcda9-114">text</span><span class="sxs-lookup"><span data-stu-id="fcda9-114">text</span></span>|<span data-ttu-id="fcda9-115">字符串</span><span class="sxs-lookup"><span data-stu-id="fcda9-115">String</span></span>|<span data-ttu-id="fcda9-116">特定语言的文本。</span><span class="sxs-lookup"><span data-stu-id="fcda9-116">The text in the specific language.</span></span> <span data-ttu-id="fcda9-117">必填。</span><span class="sxs-lookup"><span data-stu-id="fcda9-117">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fcda9-118">关系</span><span class="sxs-lookup"><span data-stu-id="fcda9-118">Relationships</span></span>
<span data-ttu-id="fcda9-119">无。</span><span class="sxs-lookup"><span data-stu-id="fcda9-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fcda9-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fcda9-120">JSON representation</span></span>
<span data-ttu-id="fcda9-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcda9-121">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageLocalizedText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageLocalizedText",
  "text": "String",
  "languageCode": "String"
}
```

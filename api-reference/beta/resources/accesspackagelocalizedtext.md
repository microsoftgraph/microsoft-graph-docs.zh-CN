---
title: accessPackageLocalizedText 资源类型
description: 用于表示特定语言中的字符串的复杂类型。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9573ae4118f02abdba5686fd94da96da71d374c2
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720134"
---
# <a name="accesspackagelocalizedtext-resource-type"></a><span data-ttu-id="3af32-103">accessPackageLocalizedText 资源类型</span><span class="sxs-lookup"><span data-stu-id="3af32-103">accessPackageLocalizedText resource type</span></span>

<span data-ttu-id="3af32-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3af32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3af32-105">用于表示特定语言中的字符串的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="3af32-105">A complex type used to represent a string in a specific language.</span></span>

## <a name="properties"></a><span data-ttu-id="3af32-106">属性</span><span class="sxs-lookup"><span data-stu-id="3af32-106">Properties</span></span>
|<span data-ttu-id="3af32-107">属性</span><span class="sxs-lookup"><span data-stu-id="3af32-107">Property</span></span>|<span data-ttu-id="3af32-108">类型</span><span class="sxs-lookup"><span data-stu-id="3af32-108">Type</span></span>|<span data-ttu-id="3af32-109">说明</span><span class="sxs-lookup"><span data-stu-id="3af32-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3af32-110">languageCode</span><span class="sxs-lookup"><span data-stu-id="3af32-110">languageCode</span></span>|<span data-ttu-id="3af32-111">String</span><span class="sxs-lookup"><span data-stu-id="3af32-111">String</span></span>|<span data-ttu-id="3af32-112">目标语言的 ISO 代码。</span><span class="sxs-lookup"><span data-stu-id="3af32-112">The ISO code for the intended language.</span></span> <span data-ttu-id="3af32-113">必需。</span><span class="sxs-lookup"><span data-stu-id="3af32-113">Required.</span></span> |
|<span data-ttu-id="3af32-114">text</span><span class="sxs-lookup"><span data-stu-id="3af32-114">text</span></span>|<span data-ttu-id="3af32-115">String</span><span class="sxs-lookup"><span data-stu-id="3af32-115">String</span></span>|<span data-ttu-id="3af32-116">特定语言的文本。</span><span class="sxs-lookup"><span data-stu-id="3af32-116">The text in the specific language.</span></span> <span data-ttu-id="3af32-117">必填。</span><span class="sxs-lookup"><span data-stu-id="3af32-117">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3af32-118">关系</span><span class="sxs-lookup"><span data-stu-id="3af32-118">Relationships</span></span>
<span data-ttu-id="3af32-119">无。</span><span class="sxs-lookup"><span data-stu-id="3af32-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3af32-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3af32-120">JSON representation</span></span>
<span data-ttu-id="3af32-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3af32-121">The following is a JSON representation of the resource.</span></span>
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

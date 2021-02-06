---
title: accessPackageLocalizedContent 资源类型
description: 用于表示不同区域设置中的文本以及默认文本的复杂类型。*
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 155d0ffd8f7f705c79bd753aa26f659968b87829
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137352"
---
# <a name="accesspackagelocalizedcontent-resource-type"></a><span data-ttu-id="6fc90-103">accessPackageLocalizedContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fc90-103">accessPackageLocalizedContent resource type</span></span>

<span data-ttu-id="6fc90-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fc90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fc90-105">用于表示多个本地化窗体中的文本的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="6fc90-105">A complex type used to represent a text in multiple localalized forms.</span></span> <span data-ttu-id="6fc90-106">它包含一个默认文本，在所请求的本地化不可用的任何情况下都使用该文本。</span><span class="sxs-lookup"><span data-stu-id="6fc90-106">It includes a default text, which is used in any case where the requested localization is not available.</span></span>

## <a name="properties"></a><span data-ttu-id="6fc90-107">属性</span><span class="sxs-lookup"><span data-stu-id="6fc90-107">Properties</span></span>
|<span data-ttu-id="6fc90-108">属性</span><span class="sxs-lookup"><span data-stu-id="6fc90-108">Property</span></span>|<span data-ttu-id="6fc90-109">类型</span><span class="sxs-lookup"><span data-stu-id="6fc90-109">Type</span></span>|<span data-ttu-id="6fc90-110">说明</span><span class="sxs-lookup"><span data-stu-id="6fc90-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fc90-111">defaultText</span><span class="sxs-lookup"><span data-stu-id="6fc90-111">defaultText</span></span>|<span data-ttu-id="6fc90-112">字符串</span><span class="sxs-lookup"><span data-stu-id="6fc90-112">String</span></span>|<span data-ttu-id="6fc90-113">回退字符串，在请求的本地化不可用时使用。</span><span class="sxs-lookup"><span data-stu-id="6fc90-113">The fallback string, which is used when a requested localization is not available.</span></span> <span data-ttu-id="6fc90-114">必填。</span><span class="sxs-lookup"><span data-stu-id="6fc90-114">Required.</span></span> |
|<span data-ttu-id="6fc90-115">localizedTexts</span><span class="sxs-lookup"><span data-stu-id="6fc90-115">localizedTexts</span></span>|<span data-ttu-id="6fc90-116">[accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6fc90-116">[accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md) collection</span></span>|<span data-ttu-id="6fc90-117">以特定区域设置的格式表示的内容。</span><span class="sxs-lookup"><span data-stu-id="6fc90-117">Content represented in a format for a specific locale.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6fc90-118">关系</span><span class="sxs-lookup"><span data-stu-id="6fc90-118">Relationships</span></span>
<span data-ttu-id="6fc90-119">无。</span><span class="sxs-lookup"><span data-stu-id="6fc90-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fc90-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fc90-120">JSON representation</span></span>
<span data-ttu-id="6fc90-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fc90-121">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageLocalizedContent",
  "defaultText": "String",
  "localizedTexts": [
    {
      "@odata.type": "microsoft.graph.accessPackageLocalizedText"
    }
  ]
}
```

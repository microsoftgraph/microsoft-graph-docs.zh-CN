---
title: accessPackageAnswer 资源类型
description: 存储在 accessPackageAssignmentRequest 上的 accessPackageQuestion 答案的复杂类型。
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3da6d1b0e2e519895af4dacca009b027807b0184
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135494"
---
# <a name="accesspackageanswer-resource-type"></a><span data-ttu-id="a04a1-103">accessPackageAnswer 资源类型</span><span class="sxs-lookup"><span data-stu-id="a04a1-103">accessPackageAnswer resource type</span></span>

<span data-ttu-id="a04a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a04a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a04a1-105">请求者提供的 [accessPackageQuestion](../resources/accesspackagequestion.md)答案的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="a04a1-105">The complex type of a requestor's provided answer to an [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span> <span data-ttu-id="a04a1-106">实际答案将是此复杂类型的子类型，[即 accessPackageAnswerString](../resources/accesspackageanswerstring.md)或[accessPackageAnswerChoice。](../resources/accesspackageanswerchoice.md)</span><span class="sxs-lookup"><span data-stu-id="a04a1-106">The actual answer will be a subtype of this complex type, either [accessPackageAnswerString](../resources/accesspackageanswerstring.md) or [accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md).</span></span> <span data-ttu-id="a04a1-107">这些答案将存储在 [accessPackageAssignmentRequest 上](../resources/accesspackageassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="a04a1-107">These answers will be stored on an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a04a1-108">属性</span><span class="sxs-lookup"><span data-stu-id="a04a1-108">Properties</span></span>
|<span data-ttu-id="a04a1-109">属性</span><span class="sxs-lookup"><span data-stu-id="a04a1-109">Property</span></span>|<span data-ttu-id="a04a1-110">类型</span><span class="sxs-lookup"><span data-stu-id="a04a1-110">Type</span></span>|<span data-ttu-id="a04a1-111">说明</span><span class="sxs-lookup"><span data-stu-id="a04a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a04a1-112">answeredQuestion</span><span class="sxs-lookup"><span data-stu-id="a04a1-112">answeredQuestion</span></span>|[<span data-ttu-id="a04a1-113">accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="a04a1-113">accessPackageQuestion</span></span>](../resources/accesspackagequestion.md)|<span data-ttu-id="a04a1-114">答案针对的问题。</span><span class="sxs-lookup"><span data-stu-id="a04a1-114">The question the answer is for.</span></span> <span data-ttu-id="a04a1-115">必需且只读。</span><span class="sxs-lookup"><span data-stu-id="a04a1-115">Required and Read-only.</span></span>|
|<span data-ttu-id="a04a1-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="a04a1-116">displayValue</span></span>|<span data-ttu-id="a04a1-117">字符串</span><span class="sxs-lookup"><span data-stu-id="a04a1-117">String</span></span>|<span data-ttu-id="a04a1-118">答案的显示值。</span><span class="sxs-lookup"><span data-stu-id="a04a1-118">The display value of the answer.</span></span> <span data-ttu-id="a04a1-119">必填。</span><span class="sxs-lookup"><span data-stu-id="a04a1-119">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a04a1-120">关系</span><span class="sxs-lookup"><span data-stu-id="a04a1-120">Relationships</span></span>
<span data-ttu-id="a04a1-121">无。</span><span class="sxs-lookup"><span data-stu-id="a04a1-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a04a1-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a04a1-122">JSON representation</span></span>
<span data-ttu-id="a04a1-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a04a1-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswer",
  "displayValue": "String",
  "answeredQuestion": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  }
}
```


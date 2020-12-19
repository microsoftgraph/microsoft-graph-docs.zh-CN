---
title: accessPackageAnswer 资源类型
description: 存储在 accessPackageAssignmentRequest 上的 accessPackageQuestion 答案的复杂类型。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f947c5235c18d3be5115199d789512602a3e0739
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720135"
---
# <a name="accesspackageanswer-resource-type"></a><span data-ttu-id="dff1a-103">accessPackageAnswer 资源类型</span><span class="sxs-lookup"><span data-stu-id="dff1a-103">accessPackageAnswer resource type</span></span>

<span data-ttu-id="dff1a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dff1a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dff1a-105">请求者提供的 [accessPackageQuestion](../resources/accesspackagequestion.md)答案的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="dff1a-105">The complex type of a requestor's provided answer to an [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span> <span data-ttu-id="dff1a-106">实际答案将是此复杂类型的子类型，[即 accessPackageAnswerString](../resources/accesspackageanswerstring.md)或[accessPackageAnswerChoice。](../resources/accesspackageanswerchoice.md)</span><span class="sxs-lookup"><span data-stu-id="dff1a-106">The actual answer will be a subtype of this complex type, either [accessPackageAnswerString](../resources/accesspackageanswerstring.md) or [accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md).</span></span> <span data-ttu-id="dff1a-107">这些答案将存储在 [accessPackageAssignmentRequest 上](../resources/accesspackageassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="dff1a-107">These answers will be stored on an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dff1a-108">属性</span><span class="sxs-lookup"><span data-stu-id="dff1a-108">Properties</span></span>
|<span data-ttu-id="dff1a-109">属性</span><span class="sxs-lookup"><span data-stu-id="dff1a-109">Property</span></span>|<span data-ttu-id="dff1a-110">类型</span><span class="sxs-lookup"><span data-stu-id="dff1a-110">Type</span></span>|<span data-ttu-id="dff1a-111">说明</span><span class="sxs-lookup"><span data-stu-id="dff1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dff1a-112">answeredQuestion</span><span class="sxs-lookup"><span data-stu-id="dff1a-112">answeredQuestion</span></span>|[<span data-ttu-id="dff1a-113">accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="dff1a-113">accessPackageQuestion</span></span>](../resources/accesspackagequestion.md)|<span data-ttu-id="dff1a-114">答案针对的问题。</span><span class="sxs-lookup"><span data-stu-id="dff1a-114">The question the answer is for.</span></span> <span data-ttu-id="dff1a-115">必需且只读。</span><span class="sxs-lookup"><span data-stu-id="dff1a-115">Required and Read-only.</span></span>|
|<span data-ttu-id="dff1a-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="dff1a-116">displayValue</span></span>|<span data-ttu-id="dff1a-117">String</span><span class="sxs-lookup"><span data-stu-id="dff1a-117">String</span></span>|<span data-ttu-id="dff1a-118">答案的显示值。</span><span class="sxs-lookup"><span data-stu-id="dff1a-118">The display value of the answer.</span></span> <span data-ttu-id="dff1a-119">必填。</span><span class="sxs-lookup"><span data-stu-id="dff1a-119">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dff1a-120">关系</span><span class="sxs-lookup"><span data-stu-id="dff1a-120">Relationships</span></span>
<span data-ttu-id="dff1a-121">无。</span><span class="sxs-lookup"><span data-stu-id="dff1a-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dff1a-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dff1a-122">JSON representation</span></span>
<span data-ttu-id="dff1a-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dff1a-123">The following is a JSON representation of the resource.</span></span>
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


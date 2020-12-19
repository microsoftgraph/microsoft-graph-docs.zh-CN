---
title: accessPackageQuestion 资源类型
description: 在访问包分配策略上配置的问题的复杂类型。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 876c21018104ed579cbaf04b0f4642395627964e
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720132"
---
# <a name="accesspackagequestion-resource-type"></a><span data-ttu-id="3df4c-103">accessPackageQuestion 资源类型</span><span class="sxs-lookup"><span data-stu-id="3df4c-103">accessPackageQuestion resource type</span></span>

<span data-ttu-id="3df4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3df4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3df4c-105">用于 `accessPackageQuestion` 访问包分配 [策略的属性](accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="3df4c-105">Used for the `accessPackageQuestion` property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> 

<span data-ttu-id="3df4c-106">子类型包括 [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) 和 [accessPackageMultipleChoiceQuestions](accesspackagemultiplechoicequestion.md)。</span><span class="sxs-lookup"><span data-stu-id="3df4c-106">Subtypes include [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) and [accessPackageMultipleChoiceQuestions](accesspackagemultiplechoicequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3df4c-107">属性</span><span class="sxs-lookup"><span data-stu-id="3df4c-107">Properties</span></span>
|<span data-ttu-id="3df4c-108">属性</span><span class="sxs-lookup"><span data-stu-id="3df4c-108">Property</span></span>|<span data-ttu-id="3df4c-109">类型</span><span class="sxs-lookup"><span data-stu-id="3df4c-109">Type</span></span>|<span data-ttu-id="3df4c-110">说明</span><span class="sxs-lookup"><span data-stu-id="3df4c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3df4c-111">id</span><span class="sxs-lookup"><span data-stu-id="3df4c-111">id</span></span>|<span data-ttu-id="3df4c-112">String</span><span class="sxs-lookup"><span data-stu-id="3df4c-112">String</span></span>| <span data-ttu-id="3df4c-113">问题的 ID。</span><span class="sxs-lookup"><span data-stu-id="3df4c-113">ID of the question.</span></span>|
|<span data-ttu-id="3df4c-114">isRequired</span><span class="sxs-lookup"><span data-stu-id="3df4c-114">isRequired</span></span>|<span data-ttu-id="3df4c-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="3df4c-115">Boolean</span></span>| <span data-ttu-id="3df4c-116">请求者是否需要提供答案。</span><span class="sxs-lookup"><span data-stu-id="3df4c-116">Whether the requestor is required to supply an answer or not.</span></span>|
|<span data-ttu-id="3df4c-117">Sequence</span><span class="sxs-lookup"><span data-stu-id="3df4c-117">sequence</span></span>|<span data-ttu-id="3df4c-118">Int32</span><span class="sxs-lookup"><span data-stu-id="3df4c-118">Int32</span></span>| <span data-ttu-id="3df4c-119">向请求者显示问题列表时此问题的相对位置。</span><span class="sxs-lookup"><span data-stu-id="3df4c-119">Relative position of this question when displaying a list of questions to the requestor.</span></span>|
|<span data-ttu-id="3df4c-120">text</span><span class="sxs-lookup"><span data-stu-id="3df4c-120">text</span></span>|[<span data-ttu-id="3df4c-121">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="3df4c-121">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="3df4c-122">要向请求者显示的问题的文本。</span><span class="sxs-lookup"><span data-stu-id="3df4c-122">The text of the question to show to the requestor.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3df4c-123">关系</span><span class="sxs-lookup"><span data-stu-id="3df4c-123">Relationships</span></span>
<span data-ttu-id="3df4c-124">无。</span><span class="sxs-lookup"><span data-stu-id="3df4c-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3df4c-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3df4c-125">JSON representation</span></span>
<span data-ttu-id="3df4c-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3df4c-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer"
}
```


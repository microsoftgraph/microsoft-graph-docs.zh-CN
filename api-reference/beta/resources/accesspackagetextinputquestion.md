---
title: accessPackageTextInputQuestion 资源类型
description: 将文本输入作为问题答案格式的 accessPackageQuestion 的子级。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8609532e096fb587b4dcf49b8eb624aea314a8c6
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720115"
---
# <a name="accesspackagetextinputquestion-resource-type"></a><span data-ttu-id="82b83-103">accessPackageTextInputQuestion 资源类型</span><span class="sxs-lookup"><span data-stu-id="82b83-103">accessPackageTextInputQuestion resource type</span></span>

<span data-ttu-id="82b83-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82b83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82b83-105">将文本输入 **作为答案的 accessPackageQuestion** 的子级。</span><span class="sxs-lookup"><span data-stu-id="82b83-105">A child of **accessPackageQuestion** that has text input as an answer.</span></span>

<span data-ttu-id="82b83-106">继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。</span><span class="sxs-lookup"><span data-stu-id="82b83-106">Inherits from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="82b83-107">属性</span><span class="sxs-lookup"><span data-stu-id="82b83-107">Properties</span></span>
|<span data-ttu-id="82b83-108">属性</span><span class="sxs-lookup"><span data-stu-id="82b83-108">Property</span></span>|<span data-ttu-id="82b83-109">类型</span><span class="sxs-lookup"><span data-stu-id="82b83-109">Type</span></span>|<span data-ttu-id="82b83-110">说明</span><span class="sxs-lookup"><span data-stu-id="82b83-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82b83-111">id</span><span class="sxs-lookup"><span data-stu-id="82b83-111">id</span></span>|<span data-ttu-id="82b83-112">String</span><span class="sxs-lookup"><span data-stu-id="82b83-112">String</span></span>|<span data-ttu-id="82b83-113">问题的 ID。</span><span class="sxs-lookup"><span data-stu-id="82b83-113">ID of the question.</span></span> <span data-ttu-id="82b83-114">继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。</span><span class="sxs-lookup"><span data-stu-id="82b83-114">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="82b83-115">isRequired</span><span class="sxs-lookup"><span data-stu-id="82b83-115">isRequired</span></span>|<span data-ttu-id="82b83-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b83-116">Boolean</span></span>|<span data-ttu-id="82b83-117">指示请求者是否需要提供答案。</span><span class="sxs-lookup"><span data-stu-id="82b83-117">Indicates whether the requestor is required to supply an answer or not.</span></span> <span data-ttu-id="82b83-118">继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。</span><span class="sxs-lookup"><span data-stu-id="82b83-118">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="82b83-119">isSingleLineQuestion</span><span class="sxs-lookup"><span data-stu-id="82b83-119">isSingleLineQuestion</span></span>|<span data-ttu-id="82b83-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b83-120">Boolean</span></span>|<span data-ttu-id="82b83-121">指示答案是单行格式还是多行格式。</span><span class="sxs-lookup"><span data-stu-id="82b83-121">Indicates whether the answer will be in single or multiple line format.</span></span>|
|<span data-ttu-id="82b83-122">Sequence</span><span class="sxs-lookup"><span data-stu-id="82b83-122">sequence</span></span>|<span data-ttu-id="82b83-123">Int32</span><span class="sxs-lookup"><span data-stu-id="82b83-123">Int32</span></span>|<span data-ttu-id="82b83-124">向请求者显示问题列表时此问题的相对位置。</span><span class="sxs-lookup"><span data-stu-id="82b83-124">Relative position of this question when displaying a list of questions to the requestor.</span></span> <span data-ttu-id="82b83-125">继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。</span><span class="sxs-lookup"><span data-stu-id="82b83-125">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="82b83-126">text</span><span class="sxs-lookup"><span data-stu-id="82b83-126">text</span></span>|[<span data-ttu-id="82b83-127">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="82b83-127">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="82b83-128">要向请求者显示的问题的文本。</span><span class="sxs-lookup"><span data-stu-id="82b83-128">The text of the question to show to the requestor.</span></span> <span data-ttu-id="82b83-129">继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。</span><span class="sxs-lookup"><span data-stu-id="82b83-129">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="82b83-130">关系</span><span class="sxs-lookup"><span data-stu-id="82b83-130">Relationships</span></span>
<span data-ttu-id="82b83-131">无。</span><span class="sxs-lookup"><span data-stu-id="82b83-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82b83-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82b83-132">JSON representation</span></span>
<span data-ttu-id="82b83-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82b83-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageTextInputQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer",
  "isSingleLineQuestion": "Boolean"
}
```


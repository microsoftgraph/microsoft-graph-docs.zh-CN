---
title: accessPackageMultipleChoiceQuestion 资源类型
description: 具有多个选项作为问题答案格式的 accessPackageQuestion 的子类
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 54054edcda2f41ad3f4e1bd29fb807c18709ee1d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137338"
---
# <a name="accesspackagemultiplechoicequestion-resource-type"></a><span data-ttu-id="499ec-103">accessPackageMultipleChoiceQuestion 资源类型</span><span class="sxs-lookup"><span data-stu-id="499ec-103">accessPackageMultipleChoiceQuestion resource type</span></span>

<span data-ttu-id="499ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="499ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="499ec-105">**accessPackageQuestion 的子项**，它提供请求者必须从中选择答案的多个选项。</span><span class="sxs-lookup"><span data-stu-id="499ec-105">A child of **accessPackageQuestion** that presents multiple options that the requestor must choose an answer from.</span></span>

<span data-ttu-id="499ec-106">继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。</span><span class="sxs-lookup"><span data-stu-id="499ec-106">Inherits from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="499ec-107">属性</span><span class="sxs-lookup"><span data-stu-id="499ec-107">Properties</span></span>
|<span data-ttu-id="499ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="499ec-108">Property</span></span>|<span data-ttu-id="499ec-109">类型</span><span class="sxs-lookup"><span data-stu-id="499ec-109">Type</span></span>|<span data-ttu-id="499ec-110">说明</span><span class="sxs-lookup"><span data-stu-id="499ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="499ec-111">allowsMultipleSelection</span><span class="sxs-lookup"><span data-stu-id="499ec-111">allowsMultipleSelection</span></span>|<span data-ttu-id="499ec-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="499ec-112">Boolean</span></span>|<span data-ttu-id="499ec-113">指示请求者是否可以选择多个选项作为其答案。</span><span class="sxs-lookup"><span data-stu-id="499ec-113">Indicates whether requestor can select multiple choices as their answer.</span></span>|
|<span data-ttu-id="499ec-114">choices</span><span class="sxs-lookup"><span data-stu-id="499ec-114">choices</span></span>|<span data-ttu-id="499ec-115">[accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499ec-115">[accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md) collection</span></span>|<span data-ttu-id="499ec-116">答案选择列表。</span><span class="sxs-lookup"><span data-stu-id="499ec-116">List of answer choices.</span></span>|
|<span data-ttu-id="499ec-117">id</span><span class="sxs-lookup"><span data-stu-id="499ec-117">id</span></span>|<span data-ttu-id="499ec-118">字符串</span><span class="sxs-lookup"><span data-stu-id="499ec-118">String</span></span>|<span data-ttu-id="499ec-119">问题的 ID。</span><span class="sxs-lookup"><span data-stu-id="499ec-119">ID of the question.</span></span> <span data-ttu-id="499ec-120">继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。</span><span class="sxs-lookup"><span data-stu-id="499ec-120">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="499ec-121">isRequired</span><span class="sxs-lookup"><span data-stu-id="499ec-121">isRequired</span></span>|<span data-ttu-id="499ec-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="499ec-122">Boolean</span></span>|<span data-ttu-id="499ec-123">指示请求者是否需要提供答案。</span><span class="sxs-lookup"><span data-stu-id="499ec-123">Indicates whether the requestor is required to supply an answer or not.</span></span> <span data-ttu-id="499ec-124">继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。</span><span class="sxs-lookup"><span data-stu-id="499ec-124">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="499ec-125">Sequence</span><span class="sxs-lookup"><span data-stu-id="499ec-125">sequence</span></span>|<span data-ttu-id="499ec-126">Int32</span><span class="sxs-lookup"><span data-stu-id="499ec-126">Int32</span></span>|<span data-ttu-id="499ec-127">向请求者显示问题列表时此问题的相对位置。</span><span class="sxs-lookup"><span data-stu-id="499ec-127">Relative position of this question when displaying a list of questions to the requestor.</span></span> <span data-ttu-id="499ec-128">继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。</span><span class="sxs-lookup"><span data-stu-id="499ec-128">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="499ec-129">text</span><span class="sxs-lookup"><span data-stu-id="499ec-129">text</span></span>|[<span data-ttu-id="499ec-130">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="499ec-130">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="499ec-131">要显示请求者的问题的文本。</span><span class="sxs-lookup"><span data-stu-id="499ec-131">The text of the question to show the requestor.</span></span> <span data-ttu-id="499ec-132">继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。</span><span class="sxs-lookup"><span data-stu-id="499ec-132">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="499ec-133">关系</span><span class="sxs-lookup"><span data-stu-id="499ec-133">Relationships</span></span>
<span data-ttu-id="499ec-134">无。</span><span class="sxs-lookup"><span data-stu-id="499ec-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="499ec-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="499ec-135">JSON representation</span></span>
<span data-ttu-id="499ec-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="499ec-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageMultipleChoiceQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer",
  "choices": [
    {
      "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
    }
  ],
  "allowsMultipleSelection": "Boolean"
}
```

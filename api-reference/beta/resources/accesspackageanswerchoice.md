---
title: accessPackageAnswerChoice 资源类型
description: accessPackageMultipleChoiceQuestion 的应答选项。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6f34656a72d217adec1ff46be689b283461332fb
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720147"
---
# <a name="accesspackageanswerchoice-resource-type"></a><span data-ttu-id="c2d6c-103">accessPackageAnswerChoice 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2d6c-103">accessPackageAnswerChoice resource type</span></span>

<span data-ttu-id="c2d6c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2d6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2d6c-105">指示 [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md)的应答选项。</span><span class="sxs-lookup"><span data-stu-id="c2d6c-105">Indicates an answer option for an [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span></span> <span data-ttu-id="c2d6c-106">可以将多个 accessPackageAnswerChoices 添加到 [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md)。</span><span class="sxs-lookup"><span data-stu-id="c2d6c-106">Multiple accessPackageAnswerChoices can be added to an [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c2d6c-107">属性</span><span class="sxs-lookup"><span data-stu-id="c2d6c-107">Properties</span></span>
|<span data-ttu-id="c2d6c-108">属性</span><span class="sxs-lookup"><span data-stu-id="c2d6c-108">Property</span></span>|<span data-ttu-id="c2d6c-109">类型</span><span class="sxs-lookup"><span data-stu-id="c2d6c-109">Type</span></span>|<span data-ttu-id="c2d6c-110">说明</span><span class="sxs-lookup"><span data-stu-id="c2d6c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2d6c-111">actualValue</span><span class="sxs-lookup"><span data-stu-id="c2d6c-111">actualValue</span></span>|<span data-ttu-id="c2d6c-112">String</span><span class="sxs-lookup"><span data-stu-id="c2d6c-112">String</span></span>|<span data-ttu-id="c2d6c-113">所选实际值的项。</span><span class="sxs-lookup"><span data-stu-id="c2d6c-113">The actual value of the selected choice.</span></span> <span data-ttu-id="c2d6c-114">这通常是应用程序可以理解的字符串值。</span><span class="sxs-lookup"><span data-stu-id="c2d6c-114">This is typically a string value which is understandable by applications.</span></span> <span data-ttu-id="c2d6c-115">必需。</span><span class="sxs-lookup"><span data-stu-id="c2d6c-115">Required.</span></span> |
|<span data-ttu-id="c2d6c-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="c2d6c-116">displayValue</span></span>|[<span data-ttu-id="c2d6c-117">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="c2d6c-117">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="c2d6c-118">向请求者和审批者显示的本地化显示值。</span><span class="sxs-lookup"><span data-stu-id="c2d6c-118">The localized display values shown to the requestor and approvers.</span></span> <span data-ttu-id="c2d6c-119">必填。</span><span class="sxs-lookup"><span data-stu-id="c2d6c-119">Required.</span></span>

## <a name="relationships"></a><span data-ttu-id="c2d6c-120">关系</span><span class="sxs-lookup"><span data-stu-id="c2d6c-120">Relationships</span></span>
<span data-ttu-id="c2d6c-121">无。</span><span class="sxs-lookup"><span data-stu-id="c2d6c-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2d6c-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2d6c-122">JSON representation</span></span>
<span data-ttu-id="c2d6c-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2d6c-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswerChoice",
  "actualValue": "String",
  "displayValue": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  }
}
```

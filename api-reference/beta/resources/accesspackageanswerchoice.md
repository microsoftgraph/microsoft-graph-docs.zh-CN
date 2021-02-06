---
title: accessPackageAnswerChoice 资源类型
description: accessPackageMultipleChoiceQuestion 的应答选项。
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7c7fc7db1c9360146c2f62fd9048ad0db3d58b80
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135476"
---
# <a name="accesspackageanswerchoice-resource-type"></a><span data-ttu-id="ee0da-103">accessPackageAnswerChoice 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee0da-103">accessPackageAnswerChoice resource type</span></span>

<span data-ttu-id="ee0da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee0da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee0da-105">指示 [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md)的应答选项。</span><span class="sxs-lookup"><span data-stu-id="ee0da-105">Indicates an answer option for an [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span></span> <span data-ttu-id="ee0da-106">可以将多个 accessPackageAnswerChoices 添加到 [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md)。</span><span class="sxs-lookup"><span data-stu-id="ee0da-106">Multiple accessPackageAnswerChoices can be added to an [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ee0da-107">属性</span><span class="sxs-lookup"><span data-stu-id="ee0da-107">Properties</span></span>
|<span data-ttu-id="ee0da-108">属性</span><span class="sxs-lookup"><span data-stu-id="ee0da-108">Property</span></span>|<span data-ttu-id="ee0da-109">类型</span><span class="sxs-lookup"><span data-stu-id="ee0da-109">Type</span></span>|<span data-ttu-id="ee0da-110">说明</span><span class="sxs-lookup"><span data-stu-id="ee0da-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee0da-111">actualValue</span><span class="sxs-lookup"><span data-stu-id="ee0da-111">actualValue</span></span>|<span data-ttu-id="ee0da-112">字符串</span><span class="sxs-lookup"><span data-stu-id="ee0da-112">String</span></span>|<span data-ttu-id="ee0da-113">所选实际值的项。</span><span class="sxs-lookup"><span data-stu-id="ee0da-113">The actual value of the selected choice.</span></span> <span data-ttu-id="ee0da-114">这通常是应用程序可以理解的字符串值。</span><span class="sxs-lookup"><span data-stu-id="ee0da-114">This is typically a string value which is understandable by applications.</span></span> <span data-ttu-id="ee0da-115">必填。</span><span class="sxs-lookup"><span data-stu-id="ee0da-115">Required.</span></span> |
|<span data-ttu-id="ee0da-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="ee0da-116">displayValue</span></span>|[<span data-ttu-id="ee0da-117">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="ee0da-117">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="ee0da-118">向请求者和审批者显示的本地化显示值。</span><span class="sxs-lookup"><span data-stu-id="ee0da-118">The localized display values shown to the requestor and approvers.</span></span> <span data-ttu-id="ee0da-119">必填。</span><span class="sxs-lookup"><span data-stu-id="ee0da-119">Required.</span></span>

## <a name="relationships"></a><span data-ttu-id="ee0da-120">关系</span><span class="sxs-lookup"><span data-stu-id="ee0da-120">Relationships</span></span>
<span data-ttu-id="ee0da-121">无。</span><span class="sxs-lookup"><span data-stu-id="ee0da-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee0da-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee0da-122">JSON representation</span></span>
<span data-ttu-id="ee0da-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee0da-123">The following is a JSON representation of the resource.</span></span>
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

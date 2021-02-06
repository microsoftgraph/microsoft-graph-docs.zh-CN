---
title: accessPackageAnswerString 资源类型
description: accessPackageTextInputQuestion 的字符串答案
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: def7753e62239e403821ed6472b3613d025942ac
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132391"
---
# <a name="accesspackageanswerstring-resource-type"></a><span data-ttu-id="293f3-103">accessPackageAnswerString 资源类型</span><span class="sxs-lookup"><span data-stu-id="293f3-103">accessPackageAnswerString resource type</span></span>

<span data-ttu-id="293f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="293f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="293f3-105">指示对 [accessPackageTextInputQuestion](../resources/accesspackagetextinputquestion.md)的字符串输入答案。</span><span class="sxs-lookup"><span data-stu-id="293f3-105">Indicates the string input answer to an [accessPackageTextInputQuestion](../resources/accesspackagetextinputquestion.md).</span></span> <span data-ttu-id="293f3-106">存储在 [accessPackageAssignmentRequest 上](../resources/accesspackageassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="293f3-106">Stored on an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span></span>

<span data-ttu-id="293f3-107">继承自 [accessPackageAnswer](../resources/accesspackageanswer.md)。</span><span class="sxs-lookup"><span data-stu-id="293f3-107">Inherits from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>

## <a name="properties"></a><span data-ttu-id="293f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="293f3-108">Properties</span></span>
|<span data-ttu-id="293f3-109">属性</span><span class="sxs-lookup"><span data-stu-id="293f3-109">Property</span></span>|<span data-ttu-id="293f3-110">类型</span><span class="sxs-lookup"><span data-stu-id="293f3-110">Type</span></span>|<span data-ttu-id="293f3-111">说明</span><span class="sxs-lookup"><span data-stu-id="293f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="293f3-112">answeredQuestion</span><span class="sxs-lookup"><span data-stu-id="293f3-112">answeredQuestion</span></span>|[<span data-ttu-id="293f3-113">accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="293f3-113">accessPackageQuestion</span></span>](../resources/accesspackagequestion.md)|<span data-ttu-id="293f3-114">答案适用的问题。</span><span class="sxs-lookup"><span data-stu-id="293f3-114">The question the answer applies to.</span></span> <span data-ttu-id="293f3-115">继承自 [accessPackageAnswer](../resources/accesspackageanswer.md)。</span><span class="sxs-lookup"><span data-stu-id="293f3-115">Inherited from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>|
|<span data-ttu-id="293f3-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="293f3-116">displayValue</span></span>|<span data-ttu-id="293f3-117">字符串</span><span class="sxs-lookup"><span data-stu-id="293f3-117">String</span></span>|<span data-ttu-id="293f3-118">向请求者和审批者显示的本地化显示值。</span><span class="sxs-lookup"><span data-stu-id="293f3-118">The localized display values shown to the requestor and approvers.</span></span> <span data-ttu-id="293f3-119">继承自 [accessPackageAnswer](../resources/accesspackageanswer.md)。</span><span class="sxs-lookup"><span data-stu-id="293f3-119">Inherited from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>|
|<span data-ttu-id="293f3-120">value</span><span class="sxs-lookup"><span data-stu-id="293f3-120">value</span></span>|<span data-ttu-id="293f3-121">String</span><span class="sxs-lookup"><span data-stu-id="293f3-121">String</span></span>|<span data-ttu-id="293f3-122">如果此答案配置为存储为特定属性，则存储在请求者用户配置文件上的值。</span><span class="sxs-lookup"><span data-stu-id="293f3-122">The value stored on the requestor's user profile, if this answer is configured to be stored as a specific attribute.</span></span>|

## <a name="relationships"></a><span data-ttu-id="293f3-123">关系</span><span class="sxs-lookup"><span data-stu-id="293f3-123">Relationships</span></span>
<span data-ttu-id="293f3-124">无。</span><span class="sxs-lookup"><span data-stu-id="293f3-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="293f3-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="293f3-125">JSON representation</span></span>
<span data-ttu-id="293f3-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="293f3-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswerString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswerString",
  "displayValue": "String",
  "answeredQuestion": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  },
  "value": "String"
}
```


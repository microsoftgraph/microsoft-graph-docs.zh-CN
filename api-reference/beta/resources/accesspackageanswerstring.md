---
title: accessPackageAnswerString 资源类型
description: accessPackageTextInputQuestion 的字符串答案
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a5273872b2ded749ddfc13998c5b0104a0a63ec
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720101"
---
# <a name="accesspackageanswerstring-resource-type"></a><span data-ttu-id="99d56-103">accessPackageAnswerString 资源类型</span><span class="sxs-lookup"><span data-stu-id="99d56-103">accessPackageAnswerString resource type</span></span>

<span data-ttu-id="99d56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99d56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99d56-105">指示 [accessPackageTextInputQuestion](../resources/accesspackagetextinputquestion.md)的字符串输入答案。</span><span class="sxs-lookup"><span data-stu-id="99d56-105">Indicates the string input answer to an [accessPackageTextInputQuestion](../resources/accesspackagetextinputquestion.md).</span></span> <span data-ttu-id="99d56-106">存储在 [accessPackageAssignmentRequest 上](../resources/accesspackageassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="99d56-106">Stored on an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span></span>

<span data-ttu-id="99d56-107">继承自 [accessPackageAnswer](../resources/accesspackageanswer.md)。</span><span class="sxs-lookup"><span data-stu-id="99d56-107">Inherits from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>

## <a name="properties"></a><span data-ttu-id="99d56-108">属性</span><span class="sxs-lookup"><span data-stu-id="99d56-108">Properties</span></span>
|<span data-ttu-id="99d56-109">属性</span><span class="sxs-lookup"><span data-stu-id="99d56-109">Property</span></span>|<span data-ttu-id="99d56-110">类型</span><span class="sxs-lookup"><span data-stu-id="99d56-110">Type</span></span>|<span data-ttu-id="99d56-111">说明</span><span class="sxs-lookup"><span data-stu-id="99d56-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99d56-112">answeredQuestion</span><span class="sxs-lookup"><span data-stu-id="99d56-112">answeredQuestion</span></span>|[<span data-ttu-id="99d56-113">accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="99d56-113">accessPackageQuestion</span></span>](../resources/accesspackagequestion.md)|<span data-ttu-id="99d56-114">答案适用的问题。</span><span class="sxs-lookup"><span data-stu-id="99d56-114">The question the answer applies to.</span></span> <span data-ttu-id="99d56-115">继承自 [accessPackageAnswer](../resources/accesspackageanswer.md)。</span><span class="sxs-lookup"><span data-stu-id="99d56-115">Inherited from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>|
|<span data-ttu-id="99d56-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="99d56-116">displayValue</span></span>|<span data-ttu-id="99d56-117">String</span><span class="sxs-lookup"><span data-stu-id="99d56-117">String</span></span>|<span data-ttu-id="99d56-118">向请求者和审批者显示的本地化显示值。</span><span class="sxs-lookup"><span data-stu-id="99d56-118">The localized display values shown to the requestor and approvers.</span></span> <span data-ttu-id="99d56-119">继承自 [accessPackageAnswer](../resources/accesspackageanswer.md)。</span><span class="sxs-lookup"><span data-stu-id="99d56-119">Inherited from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>|
|<span data-ttu-id="99d56-120">value</span><span class="sxs-lookup"><span data-stu-id="99d56-120">value</span></span>|<span data-ttu-id="99d56-121">String</span><span class="sxs-lookup"><span data-stu-id="99d56-121">String</span></span>|<span data-ttu-id="99d56-122">如果此答案配置为存储为特定属性，则存储在请求者用户配置文件上的值。</span><span class="sxs-lookup"><span data-stu-id="99d56-122">The value stored on the requestor's user profile, if this answer is configured to be stored as a specific attribute.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99d56-123">关系</span><span class="sxs-lookup"><span data-stu-id="99d56-123">Relationships</span></span>
<span data-ttu-id="99d56-124">无。</span><span class="sxs-lookup"><span data-stu-id="99d56-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="99d56-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99d56-125">JSON representation</span></span>
<span data-ttu-id="99d56-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99d56-126">The following is a JSON representation of the resource.</span></span>
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


---
title: autoReviewSettings 资源类型
description: 指定访问评审完成时的行为。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f46ef4b57a921cc08fbb8f3768597eef12c1ce4f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136930"
---
# <a name="autoreviewsettings-resource-type"></a><span data-ttu-id="e68c3-103">autoReviewSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="e68c3-103">autoReviewSettings resource type</span></span>

<span data-ttu-id="e68c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e68c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e68c3-105">**autoReviewSettings** 资源类型在 [accessReviewSettings](accessreviewsettings.md)资源中使用，并指定访问评审完成时的行为。</span><span class="sxs-lookup"><span data-stu-id="e68c3-105">The **autoReviewSettings** resource type is used in the [accessReviewSettings](accessreviewsettings.md) resource and specifies the behavior for when an access review completes.</span></span>    

## <a name="properties"></a><span data-ttu-id="e68c3-106">属性</span><span class="sxs-lookup"><span data-stu-id="e68c3-106">Properties</span></span>

| <span data-ttu-id="e68c3-107">属性</span><span class="sxs-lookup"><span data-stu-id="e68c3-107">Property</span></span> | <span data-ttu-id="e68c3-108">类型</span><span class="sxs-lookup"><span data-stu-id="e68c3-108">Type</span></span> | <span data-ttu-id="e68c3-109">说明</span><span class="sxs-lookup"><span data-stu-id="e68c3-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="e68c3-110">notReviewedResult</span><span class="sxs-lookup"><span data-stu-id="e68c3-110">notReviewedResult</span></span> | <span data-ttu-id="e68c3-111">字符串</span><span class="sxs-lookup"><span data-stu-id="e68c3-111">String</span></span> | <span data-ttu-id="e68c3-112">可能的值： `Approve` ， `Deny` 或 `Recommendation` 。</span><span class="sxs-lookup"><span data-stu-id="e68c3-112">Possible values: `Approve`, `Deny`, or `Recommendation`.</span></span>  <span data-ttu-id="e68c3-113">If `Recommendation` ， then **accessRecommendationsEnabled** in the **accessReviewSettings** resource should also be set to `true` .</span><span class="sxs-lookup"><span data-stu-id="e68c3-113">If `Recommendation`, then **accessRecommendationsEnabled** in the **accessReviewSettings** resource should also be set to `true`.</span></span> <span data-ttu-id="e68c3-114">如果希望系统提供决策，即使审阅者未做出选择，将 **accessReviewSettings** 资源中的 **autoReviewEnabled** 属性设置为包含 `true` 具有 **notReviewedResult** 属性的 **autoReviewSettings** 对象。</span><span class="sxs-lookup"><span data-stu-id="e68c3-114">If you want to have the system provide a decision even if the reviewer does not make a choice, set the **autoReviewEnabled** property in the **accessReviewSettings** resource to `true` and include an **autoReviewSettings** object with the **notReviewedResult** property.</span></span> <span data-ttu-id="e68c3-115">然后，当审阅完成时，基于 **notReviewedResult** 属性，将决定记录为或 `Approve` `Deny` 。</span><span class="sxs-lookup"><span data-stu-id="e68c3-115">Then, when a review completes, based on the **notReviewedResult** property, the decision is recorded as either `Approve` or `Deny`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e68c3-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e68c3-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.autoReviewSettings"
}-->
```json
{
  "notReviewedResult": "string"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "autoReviewSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

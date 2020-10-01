---
title: autoReviewSettings 资源类型
description: 指定访问评审完成时的行为。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b9d0a621c4229476e0b3bcdadb869e44422e931
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330318"
---
# <a name="autoreviewsettings-resource-type"></a><span data-ttu-id="98735-103">autoReviewSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="98735-103">autoReviewSettings resource type</span></span>

<span data-ttu-id="98735-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98735-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98735-105">**AutoReviewSettings**资源类型在[accessReviewSettings](accessreviewsettings.md)资源中使用，并指定访问评审完成时的行为。</span><span class="sxs-lookup"><span data-stu-id="98735-105">The **autoReviewSettings** resource type is used in the [accessReviewSettings](accessreviewsettings.md) resource and specifies the behavior for when an access review completes.</span></span>    

## <a name="properties"></a><span data-ttu-id="98735-106">属性</span><span class="sxs-lookup"><span data-stu-id="98735-106">Properties</span></span>

| <span data-ttu-id="98735-107">属性</span><span class="sxs-lookup"><span data-stu-id="98735-107">Property</span></span> | <span data-ttu-id="98735-108">类型</span><span class="sxs-lookup"><span data-stu-id="98735-108">Type</span></span> | <span data-ttu-id="98735-109">说明</span><span class="sxs-lookup"><span data-stu-id="98735-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="98735-110">notReviewedResult</span><span class="sxs-lookup"><span data-stu-id="98735-110">notReviewedResult</span></span> | <span data-ttu-id="98735-111">字符串</span><span class="sxs-lookup"><span data-stu-id="98735-111">String</span></span> | <span data-ttu-id="98735-112">可能的值： `Approve` 、 `Deny` 或 `Recommendation` 。</span><span class="sxs-lookup"><span data-stu-id="98735-112">Possible values: `Approve`, `Deny`, or `Recommendation`.</span></span>  <span data-ttu-id="98735-113">如果为 `Recommendation` ，则**accessReviewSettings**资源中的**accessRecommendationsEnabled**也应设置为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="98735-113">If `Recommendation`, then **accessRecommendationsEnabled** in the **accessReviewSettings** resource should also be set to `true`.</span></span> <span data-ttu-id="98735-114">如果您希望系统在审阅者不做出选择的情况下也提供决定，请将**accessReviewSettings**资源中的**autoReviewEnabled**属性设置为， `true` 并在**autoReviewSettings**对象中添加**notReviewedResult**属性。</span><span class="sxs-lookup"><span data-stu-id="98735-114">If you want to have the system provide a decision even if the reviewer does not make a choice, set the **autoReviewEnabled** property in the **accessReviewSettings** resource to `true` and include an **autoReviewSettings** object with the **notReviewedResult** property.</span></span> <span data-ttu-id="98735-115">然后，当评审完成时，将根据 **notReviewedResult** 属性，将决策记录为 `Approve` 或 `Deny` 。</span><span class="sxs-lookup"><span data-stu-id="98735-115">Then, when a review completes, based on the **notReviewedResult** property, the decision is recorded as either `Approve` or `Deny`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98735-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98735-116">JSON representation</span></span>

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
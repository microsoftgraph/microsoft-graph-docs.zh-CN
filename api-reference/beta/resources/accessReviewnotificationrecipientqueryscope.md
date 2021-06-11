---
title: accessReviewnotificationrecipientqueryscope 资源类型
description: 表示将接收访问评审通知的用户。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 19b619b7479212e5fc055f5ab19b025d8d512dc1
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896732"
---
# <a name="accessreviewnotificationrecipientqueryscope-resource-type"></a><span data-ttu-id="848f8-103">accessReviewnotificationrecipientqueryscope 资源类型</span><span class="sxs-lookup"><span data-stu-id="848f8-103">accessReviewnotificationrecipientqueryscope resource type</span></span>

<span data-ttu-id="848f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="848f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="848f8-105">指定收件人的静态 (例如，特定用户、组所有者或组) 接收访问评审通知。</span><span class="sxs-lookup"><span data-stu-id="848f8-105">Specifies a static list of recipients (for example, specific users, group owners, or group members) to receive access review notifications.</span></span>

<span data-ttu-id="848f8-106">继承自 [accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md)。</span><span class="sxs-lookup"><span data-stu-id="848f8-106">Inherits from [accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="848f8-107">属性</span><span class="sxs-lookup"><span data-stu-id="848f8-107">Properties</span></span>
| <span data-ttu-id="848f8-108">属性</span><span class="sxs-lookup"><span data-stu-id="848f8-108">Property</span></span> | <span data-ttu-id="848f8-109">类型</span><span class="sxs-lookup"><span data-stu-id="848f8-109">Type</span></span> | <span data-ttu-id="848f8-110">说明</span><span class="sxs-lookup"><span data-stu-id="848f8-110">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="848f8-111">查询</span><span class="sxs-lookup"><span data-stu-id="848f8-111">query</span></span> | <span data-ttu-id="848f8-112">String</span><span class="sxs-lookup"><span data-stu-id="848f8-112">String</span></span> | <span data-ttu-id="848f8-113">这表示对收件人是谁的查询。</span><span class="sxs-lookup"><span data-stu-id="848f8-113">This represents the query for who the recipients are.</span></span> <span data-ttu-id="848f8-114">例如， `/groups/{group id}/members` 对于组的成员和 `/users/{user id}` 特定用户。</span><span class="sxs-lookup"><span data-stu-id="848f8-114">For example, `/groups/{group id}/members` for group members and `/users/{user id}` for a specific user.</span></span> |
| <span data-ttu-id="848f8-115">queryType</span><span class="sxs-lookup"><span data-stu-id="848f8-115">queryType</span></span> | <span data-ttu-id="848f8-116">String</span><span class="sxs-lookup"><span data-stu-id="848f8-116">String</span></span> | <span data-ttu-id="848f8-117">指示查询的类型。</span><span class="sxs-lookup"><span data-stu-id="848f8-117">Indicates the type of query.</span></span> <span data-ttu-id="848f8-118">允许的值为 `MicrosoftGraph` 。</span><span class="sxs-lookup"><span data-stu-id="848f8-118">Allowed value is `MicrosoftGraph`.</span></span> |
| <span data-ttu-id="848f8-119">queryRoot</span><span class="sxs-lookup"><span data-stu-id="848f8-119">queryRoot</span></span> | <span data-ttu-id="848f8-120">String</span><span class="sxs-lookup"><span data-stu-id="848f8-120">String</span></span> | <span data-ttu-id="848f8-121">在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。</span><span class="sxs-lookup"><span data-stu-id="848f8-121">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="848f8-122">此属性仅在指定相对查询时是必需的，即) `./manager` 查询。</span><span class="sxs-lookup"><span data-stu-id="848f8-122">This property is only required if a relative query that is, `./manager`) is specified.</span></span> |


## <a name="relationships"></a><span data-ttu-id="848f8-123">关系</span><span class="sxs-lookup"><span data-stu-id="848f8-123">Relationships</span></span>
<span data-ttu-id="848f8-124">无。</span><span class="sxs-lookup"><span data-stu-id="848f8-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="848f8-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="848f8-125">JSON representation</span></span>
<span data-ttu-id="848f8-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="848f8-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewNotificationRecipientQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewNotificationRecipientQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```

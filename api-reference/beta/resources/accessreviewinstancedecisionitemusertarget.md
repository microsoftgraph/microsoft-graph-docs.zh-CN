---
title: accessReviewInstanceDecisionItemUserTarget 资源类型
description: 表示作为用户审阅的目标。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f10796937aa99e5808cb51bdb4069bd99d645db2
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "51469211"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a><span data-ttu-id="673ff-103">accessReviewInstanceDecisionItemUserTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="673ff-103">accessReviewInstanceDecisionItemUserTarget resource type</span></span>

<span data-ttu-id="673ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="673ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="673ff-105">表示 [accessReviewInstance 中正在审阅的用户标识](accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="673ff-105">Represents a user identity under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="673ff-106">继承自 [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md)。</span><span class="sxs-lookup"><span data-stu-id="673ff-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="673ff-107">属性</span><span class="sxs-lookup"><span data-stu-id="673ff-107">Properties</span></span>
|<span data-ttu-id="673ff-108">属性</span><span class="sxs-lookup"><span data-stu-id="673ff-108">Property</span></span>|<span data-ttu-id="673ff-109">类型</span><span class="sxs-lookup"><span data-stu-id="673ff-109">Type</span></span>|<span data-ttu-id="673ff-110">说明</span><span class="sxs-lookup"><span data-stu-id="673ff-110">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="673ff-111">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="673ff-111">userDisplayName</span></span> | <span data-ttu-id="673ff-112">String</span><span class="sxs-lookup"><span data-stu-id="673ff-112">String</span></span> | <span data-ttu-id="673ff-113">用户的名称。</span><span class="sxs-lookup"><span data-stu-id="673ff-113">The name of user.</span></span> |
| <span data-ttu-id="673ff-114">userId</span><span class="sxs-lookup"><span data-stu-id="673ff-114">userId</span></span> | <span data-ttu-id="673ff-115">String</span><span class="sxs-lookup"><span data-stu-id="673ff-115">String</span></span> | <span data-ttu-id="673ff-116">用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="673ff-116">The identifier of user.</span></span> |
| <span data-ttu-id="673ff-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="673ff-117">userPrincipalName</span></span> | <span data-ttu-id="673ff-118">String</span><span class="sxs-lookup"><span data-stu-id="673ff-118">String</span></span> | <span data-ttu-id="673ff-119">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="673ff-119">The user principal name.</span></span> |

## <a name="relationships"></a><span data-ttu-id="673ff-120">关系</span><span class="sxs-lookup"><span data-stu-id="673ff-120">Relationships</span></span>
<span data-ttu-id="673ff-121">无。</span><span class="sxs-lookup"><span data-stu-id="673ff-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="673ff-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="673ff-122">JSON representation</span></span>
<span data-ttu-id="673ff-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="673ff-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemUserTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```

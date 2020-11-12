---
title: accessReviewInstanceDecisionItemUserTarget 资源类型
description: 将评审的目标表示为用户。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aa2117895599ba1d2c4b9829b7cad22b581f2055
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000841"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a><span data-ttu-id="d8b41-103">accessReviewInstanceDecisionItemUserTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8b41-103">accessReviewInstanceDecisionItemUserTarget resource type</span></span>

<span data-ttu-id="d8b41-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8b41-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d8b41-105">代表 [accessReviewInstance](accessreviewinstance.md)中的 "审阅" 下的用户标识。</span><span class="sxs-lookup"><span data-stu-id="d8b41-105">Represents a user identity under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="d8b41-106">继承自 [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md)。</span><span class="sxs-lookup"><span data-stu-id="d8b41-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d8b41-107">属性</span><span class="sxs-lookup"><span data-stu-id="d8b41-107">Properties</span></span>
|<span data-ttu-id="d8b41-108">属性</span><span class="sxs-lookup"><span data-stu-id="d8b41-108">Property</span></span>|<span data-ttu-id="d8b41-109">类型</span><span class="sxs-lookup"><span data-stu-id="d8b41-109">Type</span></span>|<span data-ttu-id="d8b41-110">说明</span><span class="sxs-lookup"><span data-stu-id="d8b41-110">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="d8b41-111">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d8b41-111">userDisplayName</span></span> | <span data-ttu-id="d8b41-112">String</span><span class="sxs-lookup"><span data-stu-id="d8b41-112">String</span></span> | <span data-ttu-id="d8b41-113">用户的名称。</span><span class="sxs-lookup"><span data-stu-id="d8b41-113">The name of user.</span></span> |
| <span data-ttu-id="d8b41-114">userId</span><span class="sxs-lookup"><span data-stu-id="d8b41-114">userId</span></span> | <span data-ttu-id="d8b41-115">字符串</span><span class="sxs-lookup"><span data-stu-id="d8b41-115">String</span></span> | <span data-ttu-id="d8b41-116">User 的标识符。</span><span class="sxs-lookup"><span data-stu-id="d8b41-116">The identifier of user.</span></span> |
| <span data-ttu-id="d8b41-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d8b41-117">userPrincipalName</span></span> | <span data-ttu-id="d8b41-118">字符串</span><span class="sxs-lookup"><span data-stu-id="d8b41-118">String</span></span> | <span data-ttu-id="d8b41-119">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="d8b41-119">The user principal name.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d8b41-120">关系</span><span class="sxs-lookup"><span data-stu-id="d8b41-120">Relationships</span></span>
<span data-ttu-id="d8b41-121">无。</span><span class="sxs-lookup"><span data-stu-id="d8b41-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8b41-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8b41-122">JSON representation</span></span>
<span data-ttu-id="d8b41-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8b41-123">The following is a JSON representation of the resource.</span></span>
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

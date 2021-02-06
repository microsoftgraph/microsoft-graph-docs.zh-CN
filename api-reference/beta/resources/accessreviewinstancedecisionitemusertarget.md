---
title: accessReviewInstanceDecisionItemUserTarget 资源类型
description: 表示作为用户审阅的目标。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 73fba5b7329a6dd13ddc455b9ba327467dde9016
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133467"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a><span data-ttu-id="de154-103">accessReviewInstanceDecisionItemUserTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="de154-103">accessReviewInstanceDecisionItemUserTarget resource type</span></span>

<span data-ttu-id="de154-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de154-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de154-105">表示 [accessReviewInstance 中正在审查的用户标识](accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="de154-105">Represents a user identity under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="de154-106">继承自 [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md)。</span><span class="sxs-lookup"><span data-stu-id="de154-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="de154-107">属性</span><span class="sxs-lookup"><span data-stu-id="de154-107">Properties</span></span>
|<span data-ttu-id="de154-108">属性</span><span class="sxs-lookup"><span data-stu-id="de154-108">Property</span></span>|<span data-ttu-id="de154-109">类型</span><span class="sxs-lookup"><span data-stu-id="de154-109">Type</span></span>|<span data-ttu-id="de154-110">说明</span><span class="sxs-lookup"><span data-stu-id="de154-110">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="de154-111">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="de154-111">userDisplayName</span></span> | <span data-ttu-id="de154-112">String</span><span class="sxs-lookup"><span data-stu-id="de154-112">String</span></span> | <span data-ttu-id="de154-113">用户名。</span><span class="sxs-lookup"><span data-stu-id="de154-113">The name of user.</span></span> |
| <span data-ttu-id="de154-114">userId</span><span class="sxs-lookup"><span data-stu-id="de154-114">userId</span></span> | <span data-ttu-id="de154-115">字符串</span><span class="sxs-lookup"><span data-stu-id="de154-115">String</span></span> | <span data-ttu-id="de154-116">用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="de154-116">The identifier of user.</span></span> |
| <span data-ttu-id="de154-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="de154-117">userPrincipalName</span></span> | <span data-ttu-id="de154-118">字符串</span><span class="sxs-lookup"><span data-stu-id="de154-118">String</span></span> | <span data-ttu-id="de154-119">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="de154-119">The user principal name.</span></span> |

## <a name="relationships"></a><span data-ttu-id="de154-120">关系</span><span class="sxs-lookup"><span data-stu-id="de154-120">Relationships</span></span>
<span data-ttu-id="de154-121">无。</span><span class="sxs-lookup"><span data-stu-id="de154-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="de154-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de154-122">JSON representation</span></span>
<span data-ttu-id="de154-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de154-123">The following is a JSON representation of the resource.</span></span>
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

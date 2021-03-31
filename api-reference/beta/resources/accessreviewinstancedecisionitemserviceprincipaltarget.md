---
title: accessReviewInstanceDecisionItemServicePrincipalTarget 资源类型
description: 表示作为服务主体目标的审阅目标。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7d8032282d7ddaf41779b73f707b0749e3c82dd0
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "51469221"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a><span data-ttu-id="d8f73-103">accessReviewInstanceDecisionItemServicePrincipalTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8f73-103">accessReviewInstanceDecisionItemServicePrincipalTarget resource type</span></span>

<span data-ttu-id="d8f73-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8f73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="d8f73-105">表示 [accessReviewInstance 中正在审阅的服务主体](accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="d8f73-105">Represents a service principal under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="d8f73-106">继承自 [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md)。</span><span class="sxs-lookup"><span data-stu-id="d8f73-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d8f73-107">属性</span><span class="sxs-lookup"><span data-stu-id="d8f73-107">Properties</span></span>
| <span data-ttu-id="d8f73-108">属性</span><span class="sxs-lookup"><span data-stu-id="d8f73-108">Property</span></span> | <span data-ttu-id="d8f73-109">类型</span><span class="sxs-lookup"><span data-stu-id="d8f73-109">Type</span></span> | <span data-ttu-id="d8f73-110">说明</span><span class="sxs-lookup"><span data-stu-id="d8f73-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="d8f73-111">servicePrincipalID</span><span class="sxs-lookup"><span data-stu-id="d8f73-111">servicePrincipalID</span></span> | <span data-ttu-id="d8f73-112">String</span><span class="sxs-lookup"><span data-stu-id="d8f73-112">String</span></span> | <span data-ttu-id="d8f73-113">正在检查其访问权限的服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="d8f73-113">The identifier of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="d8f73-114">servicePrincipalDisplayName</span><span class="sxs-lookup"><span data-stu-id="d8f73-114">servicePrincipalDisplayName</span></span> | <span data-ttu-id="d8f73-115">String</span><span class="sxs-lookup"><span data-stu-id="d8f73-115">String</span></span> | <span data-ttu-id="d8f73-116">要显示名称访问的服务主体的组。</span><span class="sxs-lookup"><span data-stu-id="d8f73-116">The display name of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="d8f73-117">appId</span><span class="sxs-lookup"><span data-stu-id="d8f73-117">appId</span></span> | <span data-ttu-id="d8f73-118">String</span><span class="sxs-lookup"><span data-stu-id="d8f73-118">String</span></span> | <span data-ttu-id="d8f73-119">要检查的服务主体实体的 appId。</span><span class="sxs-lookup"><span data-stu-id="d8f73-119">The appId for the service principal entity being reviewed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d8f73-120">关系</span><span class="sxs-lookup"><span data-stu-id="d8f73-120">Relationships</span></span>
<span data-ttu-id="d8f73-121">无。</span><span class="sxs-lookup"><span data-stu-id="d8f73-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8f73-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8f73-122">JSON representation</span></span>
<span data-ttu-id="d8f73-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8f73-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemServicePrincipalTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemServicePrincipalTarget",
  "servicePrincipalId": "String",
  "servicePrincipalDisplayName": "String",
  "appId": "String"
}
```

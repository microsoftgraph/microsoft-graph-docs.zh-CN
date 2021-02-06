---
title: accessReviewInstanceDecisionItemServicePrincipalTarget 资源类型
description: 表示作为服务主体目标的审阅目标。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ef944fdd1b8dbe989b1ad92e3d49b1b057fdef74
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133495"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a><span data-ttu-id="48e0c-103">accessReviewInstanceDecisionItemServicePrincipalTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="48e0c-103">accessReviewInstanceDecisionItemServicePrincipalTarget resource type</span></span>

<span data-ttu-id="48e0c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48e0c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48e0c-105">表示 [accessReviewInstance 中正在审查的服务主体](accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="48e0c-105">Represents a service principal under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="48e0c-106">继承自 [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md)。</span><span class="sxs-lookup"><span data-stu-id="48e0c-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="48e0c-107">属性</span><span class="sxs-lookup"><span data-stu-id="48e0c-107">Properties</span></span>
| <span data-ttu-id="48e0c-108">属性</span><span class="sxs-lookup"><span data-stu-id="48e0c-108">Property</span></span> | <span data-ttu-id="48e0c-109">类型</span><span class="sxs-lookup"><span data-stu-id="48e0c-109">Type</span></span> | <span data-ttu-id="48e0c-110">说明</span><span class="sxs-lookup"><span data-stu-id="48e0c-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="48e0c-111">servicePrincipalID</span><span class="sxs-lookup"><span data-stu-id="48e0c-111">servicePrincipalID</span></span> | <span data-ttu-id="48e0c-112">字符串</span><span class="sxs-lookup"><span data-stu-id="48e0c-112">String</span></span> | <span data-ttu-id="48e0c-113">正在检查其访问权限的服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="48e0c-113">The identifier of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="48e0c-114">servicePrincipalDisplayName</span><span class="sxs-lookup"><span data-stu-id="48e0c-114">servicePrincipalDisplayName</span></span> | <span data-ttu-id="48e0c-115">字符串</span><span class="sxs-lookup"><span data-stu-id="48e0c-115">String</span></span> | <span data-ttu-id="48e0c-116">正在显示名称其访问权限的服务主体的组。</span><span class="sxs-lookup"><span data-stu-id="48e0c-116">The display name of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="48e0c-117">appId</span><span class="sxs-lookup"><span data-stu-id="48e0c-117">appId</span></span> | <span data-ttu-id="48e0c-118">String</span><span class="sxs-lookup"><span data-stu-id="48e0c-118">String</span></span> | <span data-ttu-id="48e0c-119">正在审查的服务主体实体的 appId。</span><span class="sxs-lookup"><span data-stu-id="48e0c-119">The appId for the service principal entity being reviewed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="48e0c-120">关系</span><span class="sxs-lookup"><span data-stu-id="48e0c-120">Relationships</span></span>
<span data-ttu-id="48e0c-121">无。</span><span class="sxs-lookup"><span data-stu-id="48e0c-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="48e0c-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48e0c-122">JSON representation</span></span>
<span data-ttu-id="48e0c-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48e0c-123">The following is a JSON representation of the resource.</span></span>
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

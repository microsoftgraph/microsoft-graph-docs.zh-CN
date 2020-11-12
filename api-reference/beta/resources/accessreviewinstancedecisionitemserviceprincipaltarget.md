---
title: accessReviewInstanceDecisionItemServicePrincipalTarget 资源类型
description: 将评审的目标表示为服务主体目标。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e9943a287dd28a44f3b36eae1a92d1b2c385496c
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000842"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a><span data-ttu-id="15d45-103">accessReviewInstanceDecisionItemServicePrincipalTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="15d45-103">accessReviewInstanceDecisionItemServicePrincipalTarget resource type</span></span>

<span data-ttu-id="15d45-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15d45-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="15d45-105">表示在 [accessReviewInstance](accessreviewinstance.md)中进行审阅的服务主体。</span><span class="sxs-lookup"><span data-stu-id="15d45-105">Represents a service principal under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="15d45-106">继承自 [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md)。</span><span class="sxs-lookup"><span data-stu-id="15d45-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="15d45-107">属性</span><span class="sxs-lookup"><span data-stu-id="15d45-107">Properties</span></span>
| <span data-ttu-id="15d45-108">属性</span><span class="sxs-lookup"><span data-stu-id="15d45-108">Property</span></span> | <span data-ttu-id="15d45-109">类型</span><span class="sxs-lookup"><span data-stu-id="15d45-109">Type</span></span> | <span data-ttu-id="15d45-110">说明</span><span class="sxs-lookup"><span data-stu-id="15d45-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="15d45-111">servicePrincipalID</span><span class="sxs-lookup"><span data-stu-id="15d45-111">servicePrincipalID</span></span> | <span data-ttu-id="15d45-112">字符串</span><span class="sxs-lookup"><span data-stu-id="15d45-112">String</span></span> | <span data-ttu-id="15d45-113">要查看其访问权限的服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="15d45-113">The identifier of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="15d45-114">servicePrincipalDisplayName</span><span class="sxs-lookup"><span data-stu-id="15d45-114">servicePrincipalDisplayName</span></span> | <span data-ttu-id="15d45-115">字符串</span><span class="sxs-lookup"><span data-stu-id="15d45-115">String</span></span> | <span data-ttu-id="15d45-116">要查看其访问权限的服务主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="15d45-116">The display name of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="15d45-117">appId</span><span class="sxs-lookup"><span data-stu-id="15d45-117">appId</span></span> | <span data-ttu-id="15d45-118">String</span><span class="sxs-lookup"><span data-stu-id="15d45-118">String</span></span> | <span data-ttu-id="15d45-119">要查看的服务主体实体的 appId。</span><span class="sxs-lookup"><span data-stu-id="15d45-119">The appId for the service principal entity being reviewed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="15d45-120">关系</span><span class="sxs-lookup"><span data-stu-id="15d45-120">Relationships</span></span>
<span data-ttu-id="15d45-121">无。</span><span class="sxs-lookup"><span data-stu-id="15d45-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="15d45-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15d45-122">JSON representation</span></span>
<span data-ttu-id="15d45-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15d45-123">The following is a JSON representation of the resource.</span></span>
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

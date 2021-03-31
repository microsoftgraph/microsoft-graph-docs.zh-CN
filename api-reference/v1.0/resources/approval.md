---
title: 审批资源类型
description: 与 userConsentRequest 关联的审批对象。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c6d41146551586f681ebf5ed7fda735151f1efc5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469541"
---
# <a name="approval-resource-type"></a><span data-ttu-id="1bb8a-103">审批资源类型</span><span class="sxs-lookup"><span data-stu-id="1bb8a-103">approval resource type</span></span>

<span data-ttu-id="1bb8a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bb8a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1bb8a-105">表示与请求关联的决策的审批对象。</span><span class="sxs-lookup"><span data-stu-id="1bb8a-105">Represents the approval object for decisions associated with a request.</span></span>

## <a name="properties"></a><span data-ttu-id="1bb8a-106">属性</span><span class="sxs-lookup"><span data-stu-id="1bb8a-106">Properties</span></span>

|<span data-ttu-id="1bb8a-107">属性</span><span class="sxs-lookup"><span data-stu-id="1bb8a-107">Property</span></span>|<span data-ttu-id="1bb8a-108">类型</span><span class="sxs-lookup"><span data-stu-id="1bb8a-108">Type</span></span>|<span data-ttu-id="1bb8a-109">说明</span><span class="sxs-lookup"><span data-stu-id="1bb8a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bb8a-110">id</span><span class="sxs-lookup"><span data-stu-id="1bb8a-110">id</span></span>|<span data-ttu-id="1bb8a-111">String</span><span class="sxs-lookup"><span data-stu-id="1bb8a-111">String</span></span>|<span data-ttu-id="1bb8a-112">审批决策的标识符。</span><span class="sxs-lookup"><span data-stu-id="1bb8a-112">Identifier of the approval decision.</span></span>|
|<span data-ttu-id="1bb8a-113">stages</span><span class="sxs-lookup"><span data-stu-id="1bb8a-113">stages</span></span>|<span data-ttu-id="1bb8a-114">[approvalStage](../resources/approvalstage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1bb8a-114">[approvalStage](../resources/approvalstage.md) collection</span></span>|<span data-ttu-id="1bb8a-115">审批决策中的阶段集合。</span><span class="sxs-lookup"><span data-stu-id="1bb8a-115">A collection of stages in the approval decision.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1bb8a-116">关系</span><span class="sxs-lookup"><span data-stu-id="1bb8a-116">Relationships</span></span>

|<span data-ttu-id="1bb8a-117">关系</span><span class="sxs-lookup"><span data-stu-id="1bb8a-117">Relationship</span></span>|<span data-ttu-id="1bb8a-118">类型</span><span class="sxs-lookup"><span data-stu-id="1bb8a-118">Type</span></span>|<span data-ttu-id="1bb8a-119">说明</span><span class="sxs-lookup"><span data-stu-id="1bb8a-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bb8a-120">stages</span><span class="sxs-lookup"><span data-stu-id="1bb8a-120">stages</span></span>|<span data-ttu-id="1bb8a-121">[approvalStage](../resources/approvalstage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1bb8a-121">[approvalStage](../resources/approvalstage.md) collection</span></span>|<span data-ttu-id="1bb8a-122">审批决策中的阶段集合。</span><span class="sxs-lookup"><span data-stu-id="1bb8a-122">A collection of stages in the approval decision.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1bb8a-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1bb8a-123">JSON representation</span></span>

<span data-ttu-id="1bb8a-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1bb8a-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.approval",
  "id": "String (identifier)",
  "stages": [{
        "@odata.type": "#microsoft.graph.approvalStage"
    }]
}
```

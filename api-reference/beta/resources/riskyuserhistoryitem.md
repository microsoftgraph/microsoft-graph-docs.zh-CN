---
title: riskyUserHistoryItem 资源类型
description: 表示 Azure AD 用户的风险历史记录
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4ae6d5fbc28e8dddb4c782aa9e9b2fad79b347ad
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442851"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="a01cb-103">riskyUserHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="a01cb-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="a01cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a01cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="a01cb-105">表示 Azure AD 用户的风险历史记录，由 Azure AD Identity Protection 确定。</span><span class="sxs-lookup"><span data-stu-id="a01cb-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> 

## <a name="methods"></a><span data-ttu-id="a01cb-106">Methods</span><span class="sxs-lookup"><span data-stu-id="a01cb-106">Methods</span></span>

| <span data-ttu-id="a01cb-107">方法</span><span class="sxs-lookup"><span data-stu-id="a01cb-107">Method</span></span>   | <span data-ttu-id="a01cb-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a01cb-108">Return Type</span></span>|<span data-ttu-id="a01cb-109">说明</span><span class="sxs-lookup"><span data-stu-id="a01cb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a01cb-110">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="a01cb-110">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="a01cb-111">[riskyUserHistoryItem](riskyuserhistoryitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a01cb-111">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="a01cb-112">获取 Azure AD 用户的风险历史记录。</span><span class="sxs-lookup"><span data-stu-id="a01cb-112">Get the risk history of an Azure AD user.</span></span>|


## <a name="properties"></a><span data-ttu-id="a01cb-113">属性</span><span class="sxs-lookup"><span data-stu-id="a01cb-113">Properties</span></span>

| <span data-ttu-id="a01cb-114">属性</span><span class="sxs-lookup"><span data-stu-id="a01cb-114">Property</span></span>       | <span data-ttu-id="a01cb-115">类型</span><span class="sxs-lookup"><span data-stu-id="a01cb-115">Type</span></span>    | <span data-ttu-id="a01cb-116">描述</span><span class="sxs-lookup"><span data-stu-id="a01cb-116">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="a01cb-117">userId</span><span class="sxs-lookup"><span data-stu-id="a01cb-117">userId</span></span>         | <span data-ttu-id="a01cb-118">string</span><span class="sxs-lookup"><span data-stu-id="a01cb-118">string</span></span>  | <span data-ttu-id="a01cb-119">用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="a01cb-119">The id of the user.</span></span> |
| <span data-ttu-id="a01cb-120">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="a01cb-120">initiatedBy</span></span>    | <span data-ttu-id="a01cb-121">bool</span><span class="sxs-lookup"><span data-stu-id="a01cb-121">bool</span></span>    | <span data-ttu-id="a01cb-122">执行该操作的主角的 ID。</span><span class="sxs-lookup"><span data-stu-id="a01cb-122">The id of actor that does the operation.</span></span> |
| <span data-ttu-id="a01cb-123">活动</span><span class="sxs-lookup"><span data-stu-id="a01cb-123">activity</span></span>       | [<span data-ttu-id="a01cb-124">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="a01cb-124">riskUserActivity</span></span>](riskuseractivity.md)| <span data-ttu-id="a01cb-125">与用户风险级别相关的活动更改。</span><span class="sxs-lookup"><span data-stu-id="a01cb-125">The activity related to user risk level change.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="a01cb-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a01cb-126">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser"
}-->

```json
{
    "userId": "string",
    "initiatedBy": "string",
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "riskyUserHistoryItem resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->



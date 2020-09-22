---
title: riskyUserHistoryItem 资源类型
description: 表示 Azure AD 用户的风险历史记录
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f91f07e889a1808696a0bfb7180b51aa06355334
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016163"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="bc841-103">riskyUserHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc841-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="bc841-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc841-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="bc841-105">表示 azure AD 用户的风险历史记录，由 Azure AD Identity Protection 确定。</span><span class="sxs-lookup"><span data-stu-id="bc841-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> 

## <a name="methods"></a><span data-ttu-id="bc841-106">方法</span><span class="sxs-lookup"><span data-stu-id="bc841-106">Methods</span></span>

| <span data-ttu-id="bc841-107">方法</span><span class="sxs-lookup"><span data-stu-id="bc841-107">Method</span></span>   | <span data-ttu-id="bc841-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="bc841-108">Return Type</span></span>|<span data-ttu-id="bc841-109">说明</span><span class="sxs-lookup"><span data-stu-id="bc841-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bc841-110">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="bc841-110">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="bc841-111">[riskyUserHistoryItem](riskyuserhistoryitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc841-111">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="bc841-112">获取 Azure AD 用户的风险历史记录。</span><span class="sxs-lookup"><span data-stu-id="bc841-112">Get the risk history of an Azure AD user.</span></span>|


## <a name="properties"></a><span data-ttu-id="bc841-113">属性</span><span class="sxs-lookup"><span data-stu-id="bc841-113">Properties</span></span>

| <span data-ttu-id="bc841-114">属性</span><span class="sxs-lookup"><span data-stu-id="bc841-114">Property</span></span>       | <span data-ttu-id="bc841-115">类型</span><span class="sxs-lookup"><span data-stu-id="bc841-115">Type</span></span>    | <span data-ttu-id="bc841-116">描述</span><span class="sxs-lookup"><span data-stu-id="bc841-116">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="bc841-117">userId</span><span class="sxs-lookup"><span data-stu-id="bc841-117">userId</span></span>         | <span data-ttu-id="bc841-118">string</span><span class="sxs-lookup"><span data-stu-id="bc841-118">string</span></span>  | <span data-ttu-id="bc841-119">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="bc841-119">The id of the user.</span></span> |
| <span data-ttu-id="bc841-120">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="bc841-120">initiatedBy</span></span>    | <span data-ttu-id="bc841-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="bc841-121">bool</span></span>    | <span data-ttu-id="bc841-122">执行此操作的主角的 id。</span><span class="sxs-lookup"><span data-stu-id="bc841-122">The id of actor that does the operation.</span></span> |
| <span data-ttu-id="bc841-123">activity</span><span class="sxs-lookup"><span data-stu-id="bc841-123">activity</span></span>       | [<span data-ttu-id="bc841-124">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="bc841-124">riskUserActivity</span></span>](riskuseractivity.md)| <span data-ttu-id="bc841-125">与用户风险级别更改相关的活动。</span><span class="sxs-lookup"><span data-stu-id="bc841-125">The activity related to user risk level change.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="bc841-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc841-126">JSON representation</span></span>

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



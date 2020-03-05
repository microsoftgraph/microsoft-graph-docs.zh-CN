---
title: riskyUserHistoryItem 资源类型
description: 表示 Azure AD 用户的风险历史记录
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 519e2a7fdb6662496cdb660095ec63ce81b849f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521052"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="7f357-103">riskyUserHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f357-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="7f357-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7f357-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="7f357-105">表示 azure AD 用户的风险历史记录，由 Azure AD Identity Protection 确定。</span><span class="sxs-lookup"><span data-stu-id="7f357-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> 

## <a name="methods"></a><span data-ttu-id="7f357-106">方法</span><span class="sxs-lookup"><span data-stu-id="7f357-106">Methods</span></span>

| <span data-ttu-id="7f357-107">方法</span><span class="sxs-lookup"><span data-stu-id="7f357-107">Method</span></span>   | <span data-ttu-id="7f357-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="7f357-108">Return Type</span></span>|<span data-ttu-id="7f357-109">说明</span><span class="sxs-lookup"><span data-stu-id="7f357-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f357-110">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="7f357-110">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="7f357-111">[riskyUserHistoryItem](riskyuserhistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="7f357-111">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="7f357-112">获取 Azure AD 用户的风险历史记录。</span><span class="sxs-lookup"><span data-stu-id="7f357-112">Get the risk history of an Azure AD user.</span></span>|


## <a name="properties"></a><span data-ttu-id="7f357-113">属性</span><span class="sxs-lookup"><span data-stu-id="7f357-113">Properties</span></span>

| <span data-ttu-id="7f357-114">属性</span><span class="sxs-lookup"><span data-stu-id="7f357-114">Property</span></span>       | <span data-ttu-id="7f357-115">类型</span><span class="sxs-lookup"><span data-stu-id="7f357-115">Type</span></span>    | <span data-ttu-id="7f357-116">说明</span><span class="sxs-lookup"><span data-stu-id="7f357-116">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="7f357-117">userId</span><span class="sxs-lookup"><span data-stu-id="7f357-117">userId</span></span>         | <span data-ttu-id="7f357-118">string</span><span class="sxs-lookup"><span data-stu-id="7f357-118">string</span></span>  | <span data-ttu-id="7f357-119">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="7f357-119">The id of the user.</span></span> |
| <span data-ttu-id="7f357-120">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="7f357-120">initiatedBy</span></span>    | <span data-ttu-id="7f357-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="7f357-121">bool</span></span>    | <span data-ttu-id="7f357-122">执行此操作的主角的 id。</span><span class="sxs-lookup"><span data-stu-id="7f357-122">The id of actor that does the operation.</span></span> |
| <span data-ttu-id="7f357-123">activity</span><span class="sxs-lookup"><span data-stu-id="7f357-123">activity</span></span>       | [<span data-ttu-id="7f357-124">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="7f357-124">riskUserActivity</span></span>](riskuseractivity.md)| <span data-ttu-id="7f357-125">与用户风险级别更改相关的活动。</span><span class="sxs-lookup"><span data-stu-id="7f357-125">The activity related to user risk level change.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="7f357-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f357-126">JSON representation</span></span>

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

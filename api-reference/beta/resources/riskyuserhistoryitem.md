---
title: riskyUserHistoryItem 资源类型
description: 表示 Azure AD 用户的风险历史记录
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 586fdb046adc8977550cc386a27284752cf487c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965332"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="3ea1c-103">riskyUserHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ea1c-103">riskyUserHistoryItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="3ea1c-104">表示 azure AD 用户的风险历史记录, 由 Azure AD Identity Protection 确定。</span><span class="sxs-lookup"><span data-stu-id="3ea1c-104">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> 

## <a name="methods"></a><span data-ttu-id="3ea1c-105">方法</span><span class="sxs-lookup"><span data-stu-id="3ea1c-105">Methods</span></span>

| <span data-ttu-id="3ea1c-106">方法</span><span class="sxs-lookup"><span data-stu-id="3ea1c-106">Method</span></span>   | <span data-ttu-id="3ea1c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="3ea1c-107">Return Type</span></span>|<span data-ttu-id="3ea1c-108">说明</span><span class="sxs-lookup"><span data-stu-id="3ea1c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3ea1c-109">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="3ea1c-109">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="3ea1c-110">[riskyUserHistoryItem](riskyuserhistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="3ea1c-110">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="3ea1c-111">获取 Azure AD 用户的风险历史记录。</span><span class="sxs-lookup"><span data-stu-id="3ea1c-111">Get the risk history of an Azure AD user.</span></span>|


## <a name="properties"></a><span data-ttu-id="3ea1c-112">属性</span><span class="sxs-lookup"><span data-stu-id="3ea1c-112">Properties</span></span>

| <span data-ttu-id="3ea1c-113">属性</span><span class="sxs-lookup"><span data-stu-id="3ea1c-113">Property</span></span>       | <span data-ttu-id="3ea1c-114">类型</span><span class="sxs-lookup"><span data-stu-id="3ea1c-114">Type</span></span>    | <span data-ttu-id="3ea1c-115">说明</span><span class="sxs-lookup"><span data-stu-id="3ea1c-115">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="3ea1c-116">userId</span><span class="sxs-lookup"><span data-stu-id="3ea1c-116">userId</span></span>         | <span data-ttu-id="3ea1c-117">string</span><span class="sxs-lookup"><span data-stu-id="3ea1c-117">string</span></span>  | <span data-ttu-id="3ea1c-118">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="3ea1c-118">The id of the user.</span></span> |
| <span data-ttu-id="3ea1c-119">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="3ea1c-119">initiatedBy</span></span>    | <span data-ttu-id="3ea1c-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="3ea1c-120">bool</span></span>    | <span data-ttu-id="3ea1c-121">执行此操作的主角的 id。</span><span class="sxs-lookup"><span data-stu-id="3ea1c-121">The id of actor that does the operation.</span></span> |
| <span data-ttu-id="3ea1c-122">activity</span><span class="sxs-lookup"><span data-stu-id="3ea1c-122">activity</span></span>       | [<span data-ttu-id="3ea1c-123">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="3ea1c-123">riskUserActivity</span></span>](riskuseractivity.md)| <span data-ttu-id="3ea1c-124">与用户风险级别更改相关的活动。</span><span class="sxs-lookup"><span data-stu-id="3ea1c-124">The activity related to user risk level change.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="3ea1c-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ea1c-125">JSON representation</span></span>

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

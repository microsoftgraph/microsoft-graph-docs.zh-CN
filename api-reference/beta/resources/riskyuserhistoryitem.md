---
title: riskyUserHistoryItem 资源类型
description: 表示 Azure AD 用户的风险历史记录
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 37f38a649aa3721e65b44e64571dafb797259cf6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33620834"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="f2901-103">riskyUserHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2901-103">riskyUserHistoryItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="f2901-104">表示 azure AD 用户的风险历史记录, 由 Azure AD Identity Protection 确定。</span><span class="sxs-lookup"><span data-stu-id="f2901-104">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> 

## <a name="methods"></a><span data-ttu-id="f2901-105">方法</span><span class="sxs-lookup"><span data-stu-id="f2901-105">Methods</span></span>

| <span data-ttu-id="f2901-106">方法</span><span class="sxs-lookup"><span data-stu-id="f2901-106">Method</span></span>   | <span data-ttu-id="f2901-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f2901-107">Return Type</span></span>|<span data-ttu-id="f2901-108">说明</span><span class="sxs-lookup"><span data-stu-id="f2901-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2901-109">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="f2901-109">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="f2901-110">[riskyUserHistoryItem](riskyuserhistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="f2901-110">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="f2901-111">获取 Azure AD 用户的风险历史记录。</span><span class="sxs-lookup"><span data-stu-id="f2901-111">Get the risk history of an Azure AD user.</span></span>|


## <a name="properties"></a><span data-ttu-id="f2901-112">属性</span><span class="sxs-lookup"><span data-stu-id="f2901-112">Properties</span></span>

| <span data-ttu-id="f2901-113">属性</span><span class="sxs-lookup"><span data-stu-id="f2901-113">Property</span></span>       | <span data-ttu-id="f2901-114">类型</span><span class="sxs-lookup"><span data-stu-id="f2901-114">Type</span></span>    | <span data-ttu-id="f2901-115">说明</span><span class="sxs-lookup"><span data-stu-id="f2901-115">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="f2901-116">userId</span><span class="sxs-lookup"><span data-stu-id="f2901-116">userId</span></span>         | <span data-ttu-id="f2901-117">string</span><span class="sxs-lookup"><span data-stu-id="f2901-117">string</span></span>  | <span data-ttu-id="f2901-118">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="f2901-118">The id of the user.</span></span> |
| <span data-ttu-id="f2901-119">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="f2901-119">initiatedBy</span></span>    | <span data-ttu-id="f2901-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="f2901-120">bool</span></span>    | <span data-ttu-id="f2901-121">执行此操作的主角的 id。</span><span class="sxs-lookup"><span data-stu-id="f2901-121">The id of actor that does the operation.</span></span> |
| <span data-ttu-id="f2901-122">activity</span><span class="sxs-lookup"><span data-stu-id="f2901-122">activity</span></span>       | [<span data-ttu-id="f2901-123">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="f2901-123">riskUserActivity</span></span>](riskuseractivity.md)| <span data-ttu-id="f2901-124">与用户风险级别更改相关的活动。</span><span class="sxs-lookup"><span data-stu-id="f2901-124">The activity related to user risk level change.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="f2901-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2901-125">JSON representation</span></span>

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

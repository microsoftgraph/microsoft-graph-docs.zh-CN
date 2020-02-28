---
title: userSet 复杂类型
description: 访问包分配策略的请求、审批和分配审阅设置中使用的类型的抽象基类型。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f23953b30918dec40f37f7809c7c024167c34132
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331395"
---
# <a name="userset-complex-type"></a><span data-ttu-id="da95f-103">userSet 复杂类型</span><span class="sxs-lookup"><span data-stu-id="da95f-103">userSet complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da95f-104">在[访问包分配策略](accesspackageassignmentpolicy.md)的请求、审批和分配审阅设置中使用。</span><span class="sxs-lookup"><span data-stu-id="da95f-104">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="da95f-105">[SingleUser](singleuser.md)、[groupMembers](groupmembers.md)、 [connectedOrganizationMembers](connectedorganizationmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md)和[externalSponsors](externalsponsors.md)类型的抽象基类型。</span><span class="sxs-lookup"><span data-stu-id="da95f-105">The abstract base type for the [singleUser](singleuser.md),[groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md), and [externalSponsors](externalsponsors.md) types.</span></span>

## <a name="properties"></a><span data-ttu-id="da95f-106">属性</span><span class="sxs-lookup"><span data-stu-id="da95f-106">Properties</span></span>

| <span data-ttu-id="da95f-107">属性</span><span class="sxs-lookup"><span data-stu-id="da95f-107">Property</span></span>                     | <span data-ttu-id="da95f-108">类型</span><span class="sxs-lookup"><span data-stu-id="da95f-108">Type</span></span>                      | <span data-ttu-id="da95f-109">说明</span><span class="sxs-lookup"><span data-stu-id="da95f-109">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="da95f-110">isBackup</span><span class="sxs-lookup"><span data-stu-id="da95f-110">isBackup</span></span> | <span data-ttu-id="da95f-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="da95f-111">Boolean</span></span> | <span data-ttu-id="da95f-112">对于审批阶段中的用户，此属性指示用户是否为备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="da95f-112">For a user in an approval stage, this property indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="da95f-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da95f-113">JSON representation</span></span>

<span data-ttu-id="da95f-114">以下是 userSet 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da95f-114">The following is a JSON representation of userSet.</span></span>  <span data-ttu-id="da95f-115">请注意，userSet 是抽象基类，因此不会发送或接收。</span><span class="sxs-lookup"><span data-stu-id="da95f-115">Note that a userSet is an abstract base class, and so would not be sent or received.</span></span>  <span data-ttu-id="da95f-116">而是将使用 " `@odata.type` `#microsoft.graph.singleUser``#microsoft.graph.groupMembers`"、""、"`#microsoft.graph.connectedOrganizationMembers`"、"`#microsoft.graph.requestorManager`"、`#microsoft.graph.internalSponsors`"" 或 "`#microsoft.graph.externalSponsors`" 中的一个。</span><span class="sxs-lookup"><span data-stu-id="da95f-116">Instead, one of the `@odata.type` of "`#microsoft.graph.singleUser`", "`#microsoft.graph.groupMembers`", "`#microsoft.graph.connectedOrganizationMembers`", "`#microsoft.graph.requestorManager`", "`#microsoft.graph.internalSponsors`" or "`#microsoft.graph.externalSponsors`" would be used.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSet",
  "baseType": ""
}-->

```json
{
       "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSet complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

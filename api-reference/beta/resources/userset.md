---
title: userSet 复杂类型
description: 访问包分配策略的请求、审批和分配审阅设置中使用的类型的抽象基类型。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 541bce7c65eaa9b284e9da5b520913b1be4ca8a3
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777712"
---
# <a name="userset-complex-type"></a><span data-ttu-id="ef723-103">userSet 复杂类型</span><span class="sxs-lookup"><span data-stu-id="ef723-103">userSet complex type</span></span>

<span data-ttu-id="ef723-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef723-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef723-105">用于访问包分配策略的请求、审批和 [分配审阅设置](accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="ef723-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="ef723-106">singleUser、groupMembers、connectedOrganizationMembers、requestorManager、internalSponsors[](internalsponsors.md)和[externalSponsors](externalsponsors.md)类型的抽象基类型。 [](singleuser.md)[](groupmembers.md) [](connectedorganizationmembers.md) [](requestormanager.md)</span><span class="sxs-lookup"><span data-stu-id="ef723-106">The abstract base type for the [singleUser](singleuser.md),[groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md), and [externalSponsors](externalsponsors.md) types.</span></span>

## <a name="properties"></a><span data-ttu-id="ef723-107">属性</span><span class="sxs-lookup"><span data-stu-id="ef723-107">Properties</span></span>

| <span data-ttu-id="ef723-108">属性</span><span class="sxs-lookup"><span data-stu-id="ef723-108">Property</span></span>                     | <span data-ttu-id="ef723-109">类型</span><span class="sxs-lookup"><span data-stu-id="ef723-109">Type</span></span>                      | <span data-ttu-id="ef723-110">说明</span><span class="sxs-lookup"><span data-stu-id="ef723-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="ef723-111">isBackup</span><span class="sxs-lookup"><span data-stu-id="ef723-111">isBackup</span></span> | <span data-ttu-id="ef723-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="ef723-112">Boolean</span></span> | <span data-ttu-id="ef723-113">对于处于审批阶段的用户，此属性指示用户是否是备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="ef723-113">For a user in an approval stage, this property indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ef723-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef723-114">JSON representation</span></span>

<span data-ttu-id="ef723-115">下面是 userSet 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef723-115">The following is a JSON representation of userSet.</span></span>  <span data-ttu-id="ef723-116">请注意，userSet 是抽象基类，因此不会发送或接收。</span><span class="sxs-lookup"><span data-stu-id="ef723-116">Note that a userSet is an abstract base class, and so would not be sent or received.</span></span>  <span data-ttu-id="ef723-117">而是使用" `@odata.type` `#microsoft.graph.singleUser` "， " `#microsoft.graph.groupMembers` "， " `#microsoft.graph.connectedOrganizationMembers` 或 `#microsoft.graph.requestorManager` " `#microsoft.graph.internalSponsors` `#microsoft.graph.externalSponsors` 之一。</span><span class="sxs-lookup"><span data-stu-id="ef723-117">Instead, one of the `@odata.type` of "`#microsoft.graph.singleUser`", "`#microsoft.graph.groupMembers`", "`#microsoft.graph.connectedOrganizationMembers`", "`#microsoft.graph.requestorManager`", "`#microsoft.graph.internalSponsors`" or "`#microsoft.graph.externalSponsors`" would be used.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSet"
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



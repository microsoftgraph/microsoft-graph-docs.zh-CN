---
title: groupMembers 复杂类型
description: 标识租户中将允许其成为请求者、审批者或审阅者的用户的集合。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0069cd6a8fd738c17a9035b519c4f141c3a5fa55
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761414"
---
# <a name="groupmembers-complex-type"></a><span data-ttu-id="63075-103">groupMembers 复杂类型</span><span class="sxs-lookup"><span data-stu-id="63075-103">groupMembers complex type</span></span>

<span data-ttu-id="63075-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63075-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63075-105">在访问包分配策略的请求、审批和分配审阅 [设置中使用](accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="63075-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="63075-106">值" " 指示此类型标识租户中将允许作为请求者、审批者或审阅者的用户集合，这些用户是特定 `@odata.type` `#microsoft.graph.groupMembers` 组的成员。</span><span class="sxs-lookup"><span data-stu-id="63075-106">The `@odata.type` value "`#microsoft.graph.groupMembers`" indicates that this type identifies a collection of users in the tenant who will be allowed as requestor, approver, or reviewer, who are the members of a specific group.</span></span>

## <a name="properties"></a><span data-ttu-id="63075-107">属性</span><span class="sxs-lookup"><span data-stu-id="63075-107">Properties</span></span>

| <span data-ttu-id="63075-108">属性</span><span class="sxs-lookup"><span data-stu-id="63075-108">Property</span></span>                     | <span data-ttu-id="63075-109">类型</span><span class="sxs-lookup"><span data-stu-id="63075-109">Type</span></span>                      | <span data-ttu-id="63075-110">说明</span><span class="sxs-lookup"><span data-stu-id="63075-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="63075-111">id</span><span class="sxs-lookup"><span data-stu-id="63075-111">id</span></span> |<span data-ttu-id="63075-112">String</span><span class="sxs-lookup"><span data-stu-id="63075-112">String</span></span> | <span data-ttu-id="63075-113">Azure AD 中组的 ID。</span><span class="sxs-lookup"><span data-stu-id="63075-113">The ID of the group in Azure AD.</span></span> |
| <span data-ttu-id="63075-114">说明</span><span class="sxs-lookup"><span data-stu-id="63075-114">description</span></span> |<span data-ttu-id="63075-115">String</span><span class="sxs-lookup"><span data-stu-id="63075-115">String</span></span> | <span data-ttu-id="63075-116">Azure AD 中的组名称。</span><span class="sxs-lookup"><span data-stu-id="63075-116">The name of the group in Azure AD.</span></span> <span data-ttu-id="63075-117">只读。</span><span class="sxs-lookup"><span data-stu-id="63075-117">Read only.</span></span> |
| <span data-ttu-id="63075-118">isBackup</span><span class="sxs-lookup"><span data-stu-id="63075-118">isBackup</span></span> | <span data-ttu-id="63075-119">布尔</span><span class="sxs-lookup"><span data-stu-id="63075-119">Boolean</span></span> | <span data-ttu-id="63075-120">对于 **处于审批阶段的 groupMembers，** 此属性指示该组的成员是备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="63075-120">For **groupMembers** in an approval stage, this property indicates that the group members are a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="63075-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63075-121">JSON representation</span></span>


<span data-ttu-id="63075-122">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63075-122">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupMembers",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "id": "string (identifier)",
  "description": "string",
  "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



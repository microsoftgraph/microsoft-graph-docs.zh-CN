---
title: groupMembers 复杂类型
description: 标识租户中将允许作为请求者、审批者或审阅者的用户的集合。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7ca1b7b0a2ae4021dc2def637e0326044ab8749e
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331375"
---
# <a name="groupmembers-complex-type"></a><span data-ttu-id="5260e-103">groupMembers 复杂类型</span><span class="sxs-lookup"><span data-stu-id="5260e-103">groupMembers complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5260e-104">在[访问包分配策略](accesspackageassignmentpolicy.md)的请求、审批和分配审阅设置中使用。</span><span class="sxs-lookup"><span data-stu-id="5260e-104">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="5260e-105">`@odata.type`值 "`#microsoft.graph.groupMembers`" 表示此类型标识租户中将允许作为特定组成员的请求者、审批者或审阅者的用户集合。</span><span class="sxs-lookup"><span data-stu-id="5260e-105">The `@odata.type` value "`#microsoft.graph.groupMembers`" indicates that this type identifies a collection of users in the tenant who will be allowed as requestor, approver, or reviewer, who are the members of a specific group.</span></span>

## <a name="properties"></a><span data-ttu-id="5260e-106">属性</span><span class="sxs-lookup"><span data-stu-id="5260e-106">Properties</span></span>

| <span data-ttu-id="5260e-107">属性</span><span class="sxs-lookup"><span data-stu-id="5260e-107">Property</span></span>                     | <span data-ttu-id="5260e-108">类型</span><span class="sxs-lookup"><span data-stu-id="5260e-108">Type</span></span>                      | <span data-ttu-id="5260e-109">说明</span><span class="sxs-lookup"><span data-stu-id="5260e-109">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="5260e-110">id</span><span class="sxs-lookup"><span data-stu-id="5260e-110">id</span></span> |<span data-ttu-id="5260e-111">字符串</span><span class="sxs-lookup"><span data-stu-id="5260e-111">String</span></span> | <span data-ttu-id="5260e-112">Azure AD 中的组 ID。</span><span class="sxs-lookup"><span data-stu-id="5260e-112">The ID of the group in Azure AD.</span></span> |
| <span data-ttu-id="5260e-113">说明</span><span class="sxs-lookup"><span data-stu-id="5260e-113">description</span></span> |<span data-ttu-id="5260e-114">String</span><span class="sxs-lookup"><span data-stu-id="5260e-114">String</span></span> | <span data-ttu-id="5260e-115">Azure AD 中的组的名称。</span><span class="sxs-lookup"><span data-stu-id="5260e-115">The name of the group in Azure AD.</span></span> <span data-ttu-id="5260e-116">只读。</span><span class="sxs-lookup"><span data-stu-id="5260e-116">Read only.</span></span> |
| <span data-ttu-id="5260e-117">isBackup</span><span class="sxs-lookup"><span data-stu-id="5260e-117">isBackup</span></span> | <span data-ttu-id="5260e-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="5260e-118">Boolean</span></span> | <span data-ttu-id="5260e-119">对于审批阶段中的**groupMembers** ，此属性指示组成员是备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="5260e-119">For **groupMembers** in an approval stage, this property indicates that the group members are a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5260e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5260e-120">JSON representation</span></span>


<span data-ttu-id="5260e-121">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5260e-121">The following is a JSON representation of the type.</span></span>

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

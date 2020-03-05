---
title: groupMembers 复杂类型
description: 标识租户中将允许作为请求者、审批者或审阅者的用户的集合。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5b4170a3baf186d907340bc1c490c508644ec30a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496934"
---
# <a name="groupmembers-complex-type"></a><span data-ttu-id="29761-103">groupMembers 复杂类型</span><span class="sxs-lookup"><span data-stu-id="29761-103">groupMembers complex type</span></span>

<span data-ttu-id="29761-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="29761-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29761-105">在[访问包分配策略](accesspackageassignmentpolicy.md)的请求、审批和分配审阅设置中使用。</span><span class="sxs-lookup"><span data-stu-id="29761-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="29761-106">`@odata.type`值 "`#microsoft.graph.groupMembers`" 表示此类型标识租户中将允许作为特定组成员的请求者、审批者或审阅者的用户集合。</span><span class="sxs-lookup"><span data-stu-id="29761-106">The `@odata.type` value "`#microsoft.graph.groupMembers`" indicates that this type identifies a collection of users in the tenant who will be allowed as requestor, approver, or reviewer, who are the members of a specific group.</span></span>

## <a name="properties"></a><span data-ttu-id="29761-107">属性</span><span class="sxs-lookup"><span data-stu-id="29761-107">Properties</span></span>

| <span data-ttu-id="29761-108">属性</span><span class="sxs-lookup"><span data-stu-id="29761-108">Property</span></span>                     | <span data-ttu-id="29761-109">类型</span><span class="sxs-lookup"><span data-stu-id="29761-109">Type</span></span>                      | <span data-ttu-id="29761-110">说明</span><span class="sxs-lookup"><span data-stu-id="29761-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="29761-111">id</span><span class="sxs-lookup"><span data-stu-id="29761-111">id</span></span> |<span data-ttu-id="29761-112">字符串</span><span class="sxs-lookup"><span data-stu-id="29761-112">String</span></span> | <span data-ttu-id="29761-113">Azure AD 中的组 ID。</span><span class="sxs-lookup"><span data-stu-id="29761-113">The ID of the group in Azure AD.</span></span> |
| <span data-ttu-id="29761-114">说明</span><span class="sxs-lookup"><span data-stu-id="29761-114">description</span></span> |<span data-ttu-id="29761-115">String</span><span class="sxs-lookup"><span data-stu-id="29761-115">String</span></span> | <span data-ttu-id="29761-116">Azure AD 中的组的名称。</span><span class="sxs-lookup"><span data-stu-id="29761-116">The name of the group in Azure AD.</span></span> <span data-ttu-id="29761-117">只读。</span><span class="sxs-lookup"><span data-stu-id="29761-117">Read only.</span></span> |
| <span data-ttu-id="29761-118">isBackup</span><span class="sxs-lookup"><span data-stu-id="29761-118">isBackup</span></span> | <span data-ttu-id="29761-119">布尔</span><span class="sxs-lookup"><span data-stu-id="29761-119">Boolean</span></span> | <span data-ttu-id="29761-120">对于审批阶段中的**groupMembers** ，此属性指示组成员是备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="29761-120">For **groupMembers** in an approval stage, this property indicates that the group members are a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="29761-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29761-121">JSON representation</span></span>


<span data-ttu-id="29761-122">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29761-122">The following is a JSON representation of the type.</span></span>

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

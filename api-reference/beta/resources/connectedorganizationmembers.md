---
title: connectedOrganizationMembers 复杂类型
description: ConnectedOrganizationMembers 类型标识租户中将允许作为请求者、审批者或审阅者的用户的集合。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 20f4477998547d6e98572fd8409f69e811c2198d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507490"
---
# <a name="connectedorganizationmembers-complex-type"></a><span data-ttu-id="a55ed-103">connectedOrganizationMembers 复杂类型</span><span class="sxs-lookup"><span data-stu-id="a55ed-103">connectedOrganizationMembers complex type</span></span>

<span data-ttu-id="a55ed-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a55ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a55ed-105">在[访问包分配策略](accesspackageassignmentpolicy.md)的请求设置中使用。</span><span class="sxs-lookup"><span data-stu-id="a55ed-105">Used in the request settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="a55ed-106">`@odata.type`该值`#microsoft.graph.connectedOrganizationMembers`指示此类型标识用户的集合，这些用户与已连接的组织相关联，将允许其请求访问包。</span><span class="sxs-lookup"><span data-stu-id="a55ed-106">The `@odata.type` value `#microsoft.graph.connectedOrganizationMembers` indicates that this type identifies a collection of users, those who are associated with a connected organization, who will be allowed to request an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="a55ed-107">属性</span><span class="sxs-lookup"><span data-stu-id="a55ed-107">Properties</span></span>

<span data-ttu-id="a55ed-108">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="a55ed-108">This type has the following properties:</span></span>

| <span data-ttu-id="a55ed-109">属性</span><span class="sxs-lookup"><span data-stu-id="a55ed-109">Property</span></span>                     | <span data-ttu-id="a55ed-110">类型</span><span class="sxs-lookup"><span data-stu-id="a55ed-110">Type</span></span>                      | <span data-ttu-id="a55ed-111">说明</span><span class="sxs-lookup"><span data-stu-id="a55ed-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="a55ed-112">id</span><span class="sxs-lookup"><span data-stu-id="a55ed-112">id</span></span> |<span data-ttu-id="a55ed-113">字符串</span><span class="sxs-lookup"><span data-stu-id="a55ed-113">String</span></span> | <span data-ttu-id="a55ed-114">在 "权限管理" 中连接的组织的 ID。</span><span class="sxs-lookup"><span data-stu-id="a55ed-114">The ID of the connected organization in entitlement management.</span></span> |
| <span data-ttu-id="a55ed-115">说明</span><span class="sxs-lookup"><span data-stu-id="a55ed-115">description</span></span> |<span data-ttu-id="a55ed-116">String</span><span class="sxs-lookup"><span data-stu-id="a55ed-116">String</span></span> | <span data-ttu-id="a55ed-117">连接的组织的名称。</span><span class="sxs-lookup"><span data-stu-id="a55ed-117">The name of the connected organization.</span></span> <span data-ttu-id="a55ed-118">只读。</span><span class="sxs-lookup"><span data-stu-id="a55ed-118">Read only.</span></span> |
| <span data-ttu-id="a55ed-119">isBackup</span><span class="sxs-lookup"><span data-stu-id="a55ed-119">isBackup</span></span> | <span data-ttu-id="a55ed-120">布尔</span><span class="sxs-lookup"><span data-stu-id="a55ed-120">Boolean</span></span> | <span data-ttu-id="a55ed-121">目前未使用。</span><span class="sxs-lookup"><span data-stu-id="a55ed-121">Not used at present.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a55ed-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a55ed-122">JSON representation</span></span>

<span data-ttu-id="a55ed-123">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a55ed-123">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectedOrganizationMembers",
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
  "description": "connectedOrganizationMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

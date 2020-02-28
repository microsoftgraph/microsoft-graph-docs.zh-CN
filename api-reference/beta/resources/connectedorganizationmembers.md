---
title: connectedOrganizationMembers 复杂类型
description: ConnectedOrganizationMembers 类型标识租户中将允许作为请求者、审批者或审阅者的用户的集合。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f2a3b55e3fab41f0fe08fcf844a6d143b12d7146
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331391"
---
# <a name="connectedorganizationmembers-complex-type"></a><span data-ttu-id="124d5-103">connectedOrganizationMembers 复杂类型</span><span class="sxs-lookup"><span data-stu-id="124d5-103">connectedOrganizationMembers complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="124d5-104">在[访问包分配策略](accesspackageassignmentpolicy.md)的请求设置中使用。</span><span class="sxs-lookup"><span data-stu-id="124d5-104">Used in the request settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="124d5-105">`@odata.type`该值`#microsoft.graph.connectedOrganizationMembers`指示此类型标识用户的集合，这些用户与已连接的组织相关联，将允许其请求访问包。</span><span class="sxs-lookup"><span data-stu-id="124d5-105">The `@odata.type` value `#microsoft.graph.connectedOrganizationMembers` indicates that this type identifies a collection of users, those who are associated with a connected organization, who will be allowed to request an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="124d5-106">属性</span><span class="sxs-lookup"><span data-stu-id="124d5-106">Properties</span></span>

<span data-ttu-id="124d5-107">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="124d5-107">This type has the following properties:</span></span>

| <span data-ttu-id="124d5-108">属性</span><span class="sxs-lookup"><span data-stu-id="124d5-108">Property</span></span>                     | <span data-ttu-id="124d5-109">类型</span><span class="sxs-lookup"><span data-stu-id="124d5-109">Type</span></span>                      | <span data-ttu-id="124d5-110">说明</span><span class="sxs-lookup"><span data-stu-id="124d5-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="124d5-111">id</span><span class="sxs-lookup"><span data-stu-id="124d5-111">id</span></span> |<span data-ttu-id="124d5-112">字符串</span><span class="sxs-lookup"><span data-stu-id="124d5-112">String</span></span> | <span data-ttu-id="124d5-113">在 "权限管理" 中连接的组织的 ID。</span><span class="sxs-lookup"><span data-stu-id="124d5-113">The ID of the connected organization in entitlement management.</span></span> |
| <span data-ttu-id="124d5-114">说明</span><span class="sxs-lookup"><span data-stu-id="124d5-114">description</span></span> |<span data-ttu-id="124d5-115">String</span><span class="sxs-lookup"><span data-stu-id="124d5-115">String</span></span> | <span data-ttu-id="124d5-116">连接的组织的名称。</span><span class="sxs-lookup"><span data-stu-id="124d5-116">The name of the connected organization.</span></span> <span data-ttu-id="124d5-117">只读。</span><span class="sxs-lookup"><span data-stu-id="124d5-117">Read only.</span></span> |
| <span data-ttu-id="124d5-118">isBackup</span><span class="sxs-lookup"><span data-stu-id="124d5-118">isBackup</span></span> | <span data-ttu-id="124d5-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="124d5-119">Boolean</span></span> | <span data-ttu-id="124d5-120">目前未使用。</span><span class="sxs-lookup"><span data-stu-id="124d5-120">Not used at present.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="124d5-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="124d5-121">JSON representation</span></span>

<span data-ttu-id="124d5-122">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="124d5-122">The following is a JSON representation of the type.</span></span>

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

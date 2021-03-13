---
title: connectedOrganizationMembers 复杂类型
description: connectedOrganizationMembers 类型标识租户中将允许其成为请求者、审批者或审阅者的用户的集合。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 725926bc39583bda653294f0cc917ea7d2f08a45
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761812"
---
# <a name="connectedorganizationmembers-complex-type"></a><span data-ttu-id="d7c6f-103">connectedOrganizationMembers 复杂类型</span><span class="sxs-lookup"><span data-stu-id="d7c6f-103">connectedOrganizationMembers complex type</span></span>

<span data-ttu-id="d7c6f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7c6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7c6f-105">在访问包分配策略 [的请求设置中使用](accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="d7c6f-105">Used in the request settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="d7c6f-106">值指示此类型标识用户的集合，即与已连接组织关联的用户，将允许这些用户 `@odata.type` `#microsoft.graph.connectedOrganizationMembers` 请求访问包。 [](connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="d7c6f-106">The `@odata.type` value `#microsoft.graph.connectedOrganizationMembers` indicates that this type identifies a collection of users, those who are associated with a [connected organization](connectedorganization.md), who will be allowed to request an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="d7c6f-107">属性</span><span class="sxs-lookup"><span data-stu-id="d7c6f-107">Properties</span></span>

<span data-ttu-id="d7c6f-108">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="d7c6f-108">This type has the following properties:</span></span>

| <span data-ttu-id="d7c6f-109">属性</span><span class="sxs-lookup"><span data-stu-id="d7c6f-109">Property</span></span>                     | <span data-ttu-id="d7c6f-110">类型</span><span class="sxs-lookup"><span data-stu-id="d7c6f-110">Type</span></span>                      | <span data-ttu-id="d7c6f-111">说明</span><span class="sxs-lookup"><span data-stu-id="d7c6f-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="d7c6f-112">id</span><span class="sxs-lookup"><span data-stu-id="d7c6f-112">id</span></span> |<span data-ttu-id="d7c6f-113">String</span><span class="sxs-lookup"><span data-stu-id="d7c6f-113">String</span></span> | <span data-ttu-id="d7c6f-114">权利管理中连接的组织的 ID。</span><span class="sxs-lookup"><span data-stu-id="d7c6f-114">The ID of the connected organization in entitlement management.</span></span> |
| <span data-ttu-id="d7c6f-115">说明</span><span class="sxs-lookup"><span data-stu-id="d7c6f-115">description</span></span> |<span data-ttu-id="d7c6f-116">String</span><span class="sxs-lookup"><span data-stu-id="d7c6f-116">String</span></span> | <span data-ttu-id="d7c6f-117">已连接组织的名称。</span><span class="sxs-lookup"><span data-stu-id="d7c6f-117">The name of the connected organization.</span></span> <span data-ttu-id="d7c6f-118">只读。</span><span class="sxs-lookup"><span data-stu-id="d7c6f-118">Read only.</span></span> |
| <span data-ttu-id="d7c6f-119">isBackup</span><span class="sxs-lookup"><span data-stu-id="d7c6f-119">isBackup</span></span> | <span data-ttu-id="d7c6f-120">布尔</span><span class="sxs-lookup"><span data-stu-id="d7c6f-120">Boolean</span></span> | <span data-ttu-id="d7c6f-121">目前未使用。</span><span class="sxs-lookup"><span data-stu-id="d7c6f-121">Not used at present.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d7c6f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7c6f-122">JSON representation</span></span>

<span data-ttu-id="d7c6f-123">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7c6f-123">The following is a JSON representation of the type.</span></span>

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



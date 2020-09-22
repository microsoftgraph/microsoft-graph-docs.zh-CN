---
title: connectedOrganizationMembers 复杂类型
description: ConnectedOrganizationMembers 类型标识租户中将允许作为请求者、审批者或审阅者的用户的集合。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d2df6b91ebcbc65f03ee39103768bdfad04df62f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027193"
---
# <a name="connectedorganizationmembers-complex-type"></a><span data-ttu-id="857f5-103">connectedOrganizationMembers 复杂类型</span><span class="sxs-lookup"><span data-stu-id="857f5-103">connectedOrganizationMembers complex type</span></span>

<span data-ttu-id="857f5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="857f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="857f5-105">在 [访问包分配策略](accesspackageassignmentpolicy.md)的请求设置中使用。</span><span class="sxs-lookup"><span data-stu-id="857f5-105">Used in the request settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="857f5-106">`@odata.type`该值 `#microsoft.graph.connectedOrganizationMembers` 指示此类型标识用户的集合，这些用户与[已连接的组织](connectedorganization.md)相关联，将允许其请求访问包。</span><span class="sxs-lookup"><span data-stu-id="857f5-106">The `@odata.type` value `#microsoft.graph.connectedOrganizationMembers` indicates that this type identifies a collection of users, those who are associated with a [connected organization](connectedorganization.md), who will be allowed to request an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="857f5-107">属性</span><span class="sxs-lookup"><span data-stu-id="857f5-107">Properties</span></span>

<span data-ttu-id="857f5-108">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="857f5-108">This type has the following properties:</span></span>

| <span data-ttu-id="857f5-109">属性</span><span class="sxs-lookup"><span data-stu-id="857f5-109">Property</span></span>                     | <span data-ttu-id="857f5-110">类型</span><span class="sxs-lookup"><span data-stu-id="857f5-110">Type</span></span>                      | <span data-ttu-id="857f5-111">说明</span><span class="sxs-lookup"><span data-stu-id="857f5-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="857f5-112">id</span><span class="sxs-lookup"><span data-stu-id="857f5-112">id</span></span> |<span data-ttu-id="857f5-113">String</span><span class="sxs-lookup"><span data-stu-id="857f5-113">String</span></span> | <span data-ttu-id="857f5-114">在 "权限管理" 中连接的组织的 ID。</span><span class="sxs-lookup"><span data-stu-id="857f5-114">The ID of the connected organization in entitlement management.</span></span> |
| <span data-ttu-id="857f5-115">description</span><span class="sxs-lookup"><span data-stu-id="857f5-115">description</span></span> |<span data-ttu-id="857f5-116">String</span><span class="sxs-lookup"><span data-stu-id="857f5-116">String</span></span> | <span data-ttu-id="857f5-117">连接的组织的名称。</span><span class="sxs-lookup"><span data-stu-id="857f5-117">The name of the connected organization.</span></span> <span data-ttu-id="857f5-118">只读。</span><span class="sxs-lookup"><span data-stu-id="857f5-118">Read only.</span></span> |
| <span data-ttu-id="857f5-119">isBackup</span><span class="sxs-lookup"><span data-stu-id="857f5-119">isBackup</span></span> | <span data-ttu-id="857f5-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="857f5-120">Boolean</span></span> | <span data-ttu-id="857f5-121">目前未使用。</span><span class="sxs-lookup"><span data-stu-id="857f5-121">Not used at present.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="857f5-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="857f5-122">JSON representation</span></span>

<span data-ttu-id="857f5-123">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="857f5-123">The following is a JSON representation of the type.</span></span>

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



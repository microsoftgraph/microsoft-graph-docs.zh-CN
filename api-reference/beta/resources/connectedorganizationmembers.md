---
title: connectedOrganizationMembers 复杂类型
description: ConnectedOrganizationMembers 类型标识租户中将允许作为请求者、审批者或审阅者的用户的集合。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7eddc19d3d802174ca015877ec362ec742f2e791
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509797"
---
# <a name="connectedorganizationmembers-complex-type"></a><span data-ttu-id="a4a2b-103">connectedOrganizationMembers 复杂类型</span><span class="sxs-lookup"><span data-stu-id="a4a2b-103">connectedOrganizationMembers complex type</span></span>

<span data-ttu-id="a4a2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4a2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4a2b-105">在[访问包分配策略](accesspackageassignmentpolicy.md)的请求设置中使用。</span><span class="sxs-lookup"><span data-stu-id="a4a2b-105">Used in the request settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="a4a2b-106">`@odata.type`该值 `#microsoft.graph.connectedOrganizationMembers` 指示此类型标识用户的集合，这些用户与[已连接的组织](connectedorganization.md)相关联，将允许其请求访问包。</span><span class="sxs-lookup"><span data-stu-id="a4a2b-106">The `@odata.type` value `#microsoft.graph.connectedOrganizationMembers` indicates that this type identifies a collection of users, those who are associated with a [connected organization](connectedorganization.md), who will be allowed to request an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="a4a2b-107">属性</span><span class="sxs-lookup"><span data-stu-id="a4a2b-107">Properties</span></span>

<span data-ttu-id="a4a2b-108">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="a4a2b-108">This type has the following properties:</span></span>

| <span data-ttu-id="a4a2b-109">属性</span><span class="sxs-lookup"><span data-stu-id="a4a2b-109">Property</span></span>                     | <span data-ttu-id="a4a2b-110">类型</span><span class="sxs-lookup"><span data-stu-id="a4a2b-110">Type</span></span>                      | <span data-ttu-id="a4a2b-111">说明</span><span class="sxs-lookup"><span data-stu-id="a4a2b-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="a4a2b-112">id</span><span class="sxs-lookup"><span data-stu-id="a4a2b-112">id</span></span> |<span data-ttu-id="a4a2b-113">字符串</span><span class="sxs-lookup"><span data-stu-id="a4a2b-113">String</span></span> | <span data-ttu-id="a4a2b-114">在 "权限管理" 中连接的组织的 ID。</span><span class="sxs-lookup"><span data-stu-id="a4a2b-114">The ID of the connected organization in entitlement management.</span></span> |
| <span data-ttu-id="a4a2b-115">说明</span><span class="sxs-lookup"><span data-stu-id="a4a2b-115">description</span></span> |<span data-ttu-id="a4a2b-116">String</span><span class="sxs-lookup"><span data-stu-id="a4a2b-116">String</span></span> | <span data-ttu-id="a4a2b-117">连接的组织的名称。</span><span class="sxs-lookup"><span data-stu-id="a4a2b-117">The name of the connected organization.</span></span> <span data-ttu-id="a4a2b-118">只读。</span><span class="sxs-lookup"><span data-stu-id="a4a2b-118">Read only.</span></span> |
| <span data-ttu-id="a4a2b-119">isBackup</span><span class="sxs-lookup"><span data-stu-id="a4a2b-119">isBackup</span></span> | <span data-ttu-id="a4a2b-120">布尔</span><span class="sxs-lookup"><span data-stu-id="a4a2b-120">Boolean</span></span> | <span data-ttu-id="a4a2b-121">目前未使用。</span><span class="sxs-lookup"><span data-stu-id="a4a2b-121">Not used at present.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a4a2b-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4a2b-122">JSON representation</span></span>

<span data-ttu-id="a4a2b-123">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4a2b-123">The following is a JSON representation of the type.</span></span>

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

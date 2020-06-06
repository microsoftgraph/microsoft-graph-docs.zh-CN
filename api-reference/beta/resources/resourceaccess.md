---
title: resourceAccess 资源类型
description: 指定应用程序所需的 OAuth 2.0 权限范围或应用程序角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 6092a427a2882c4b6bdae07bb98f8bc8a81eecfb
ms.sourcegitcommit: 53a57f19a5b16029b540e61ddfba6c2b4e45cfc5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2020
ms.locfileid: "44593630"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="84c6e-103">resourceAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="84c6e-103">resourceAccess resource type</span></span>

<span data-ttu-id="84c6e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84c6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84c6e-105">指定应用程序所需的 OAuth 2.0 权限范围或应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="84c6e-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="84c6e-106">[RequiredResourceAccess](requiredresourceaccess.md)类型的**ResourceAccess**属性是**resourceAccess**的集合。</span><span class="sxs-lookup"><span data-stu-id="84c6e-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>

## <a name="properties"></a><span data-ttu-id="84c6e-107">属性</span><span class="sxs-lookup"><span data-stu-id="84c6e-107">Properties</span></span>
| <span data-ttu-id="84c6e-108">属性</span><span class="sxs-lookup"><span data-stu-id="84c6e-108">Property</span></span>     | <span data-ttu-id="84c6e-109">类型</span><span class="sxs-lookup"><span data-stu-id="84c6e-109">Type</span></span>   |<span data-ttu-id="84c6e-110">说明</span><span class="sxs-lookup"><span data-stu-id="84c6e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84c6e-111">id</span><span class="sxs-lookup"><span data-stu-id="84c6e-111">id</span></span>|<span data-ttu-id="84c6e-112">Guid</span><span class="sxs-lookup"><span data-stu-id="84c6e-112">Guid</span></span>|<span data-ttu-id="84c6e-113">资源应用程序公开的[oauth2PermissionScopes](permissionscope.md)或[appRole](approle.md)实例之一的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="84c6e-113">The unique identifier for one of the [oauth2PermissionScopes](permissionscope.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="84c6e-114">type</span><span class="sxs-lookup"><span data-stu-id="84c6e-114">type</span></span>|<span data-ttu-id="84c6e-115">String</span><span class="sxs-lookup"><span data-stu-id="84c6e-115">String</span></span>|<span data-ttu-id="84c6e-116">指定**id**属性引用的是[oauth2PermissionScopes](permissionscope.md)还是[appRole](approle.md)。</span><span class="sxs-lookup"><span data-stu-id="84c6e-116">Specifies whether the **id** property references an [oauth2PermissionScopes](permissionscope.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="84c6e-117">可能的值为 `Scope` 或 `Role` 。</span><span class="sxs-lookup"><span data-stu-id="84c6e-117">Possible values are `Scope` or `Role`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84c6e-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84c6e-118">JSON representation</span></span>

<span data-ttu-id="84c6e-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84c6e-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

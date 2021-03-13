---
title: resourceAccess 资源类型
description: 指定 OAuth 2.0 权限范围或应用程序所需的应用程序角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 0072bf231fe8dba66b34188952804083593afaa1
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761070"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="e8191-103">resourceAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8191-103">resourceAccess resource type</span></span>

<span data-ttu-id="e8191-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8191-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8191-105">指定 OAuth 2.0 权限范围或应用程序所需的应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="e8191-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="e8191-106">**requiredResourceAccess** 类型的 [resourceAccess](requiredresourceaccess.md)属性是 **ResourceAccess 的集合**。</span><span class="sxs-lookup"><span data-stu-id="e8191-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>

## <a name="properties"></a><span data-ttu-id="e8191-107">属性</span><span class="sxs-lookup"><span data-stu-id="e8191-107">Properties</span></span>
| <span data-ttu-id="e8191-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8191-108">Property</span></span>     | <span data-ttu-id="e8191-109">类型</span><span class="sxs-lookup"><span data-stu-id="e8191-109">Type</span></span>   |<span data-ttu-id="e8191-110">说明</span><span class="sxs-lookup"><span data-stu-id="e8191-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8191-111">id</span><span class="sxs-lookup"><span data-stu-id="e8191-111">id</span></span>|<span data-ttu-id="e8191-112">Guid</span><span class="sxs-lookup"><span data-stu-id="e8191-112">Guid</span></span>|<span data-ttu-id="e8191-113">资源应用程序公开其中一个 [oauth2PermissionScopes](permissionscope.md) 或 [appRole](approle.md) 实例的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e8191-113">The unique identifier for one of the [oauth2PermissionScopes](permissionscope.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="e8191-114">type</span><span class="sxs-lookup"><span data-stu-id="e8191-114">type</span></span>|<span data-ttu-id="e8191-115">String</span><span class="sxs-lookup"><span data-stu-id="e8191-115">String</span></span>|<span data-ttu-id="e8191-116">指定 id **属性引用** [oauth2PermissionScopes](permissionscope.md) 还是 [appRole](approle.md)。</span><span class="sxs-lookup"><span data-stu-id="e8191-116">Specifies whether the **id** property references an [oauth2PermissionScopes](permissionscope.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="e8191-117">可能的值为 `Scope` 或 `Role`。</span><span class="sxs-lookup"><span data-stu-id="e8191-117">Possible values are `Scope` or `Role`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8191-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8191-118">JSON representation</span></span>

<span data-ttu-id="e8191-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8191-119">The following is a JSON representation of the resource.</span></span>

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



---
title: resourceAccess 资源类型
description: 指定应用程序所需的 OAuth 2.0 权限范围或应用程序角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: d0d04ba99c0132a0f305bb0fdcaa5e32071d7554
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939262"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="9aa95-103">resourceAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="9aa95-103">resourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9aa95-104">指定应用程序所需的 OAuth 2.0 权限范围或应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="9aa95-104">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="9aa95-105">[RequiredResourceAccess](requiredresourceaccess.md)类型的**ResourceAccess**属性是**resourceAccess**的集合。</span><span class="sxs-lookup"><span data-stu-id="9aa95-105">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9aa95-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9aa95-106">JSON representation</span></span>

<span data-ttu-id="9aa95-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9aa95-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="9aa95-108">属性</span><span class="sxs-lookup"><span data-stu-id="9aa95-108">Properties</span></span>
| <span data-ttu-id="9aa95-109">属性</span><span class="sxs-lookup"><span data-stu-id="9aa95-109">Property</span></span>     | <span data-ttu-id="9aa95-110">类型</span><span class="sxs-lookup"><span data-stu-id="9aa95-110">Type</span></span>   |<span data-ttu-id="9aa95-111">说明</span><span class="sxs-lookup"><span data-stu-id="9aa95-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9aa95-112">id</span><span class="sxs-lookup"><span data-stu-id="9aa95-112">id</span></span>|<span data-ttu-id="9aa95-113">Guid</span><span class="sxs-lookup"><span data-stu-id="9aa95-113">Guid</span></span>|<span data-ttu-id="9aa95-114">资源应用程序公开的[oauth2PermissionScopes](permissionscope.md)或[appRole](approle.md)实例之一的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9aa95-114">The unique identifier for one of the [oauth2PermissionScopes](permissionscope.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="9aa95-115">type</span><span class="sxs-lookup"><span data-stu-id="9aa95-115">type</span></span>|<span data-ttu-id="9aa95-116">字符串</span><span class="sxs-lookup"><span data-stu-id="9aa95-116">String</span></span>|<span data-ttu-id="9aa95-117">指定**id**属性引用的是[oauth2PermissionScopes](permissionscope.md)还是[appRole](approle.md)。</span><span class="sxs-lookup"><span data-stu-id="9aa95-117">Specifies whether the **id** property references an [oauth2PermissionScopes](permissionscope.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="9aa95-118">可能的值为 "scope" 或 "role"。</span><span class="sxs-lookup"><span data-stu-id="9aa95-118">Possible values are "scope" or "role".</span></span>|

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

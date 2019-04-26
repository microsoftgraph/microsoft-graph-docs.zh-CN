---
title: resourceAccess 资源类型
description: 指定应用程序所需的 OAuth 2.0 权限范围或应用程序角色。 requiredResourceAccess 类型的**resourceAccess**属性是**resourceAccess**的集合。
localization_priority: Normal
ms.openlocfilehash: bb77a12a207e274b27263029d96f4ef260cfe5cb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343631"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="fddd3-104">resourceAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="fddd3-104">resourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fddd3-105">指定应用程序所需的 OAuth 2.0 权限范围或应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="fddd3-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="fddd3-106">[requiredResourceAccess](requiredresourceaccess.md)类型的**resourceAccess**属性是**resourceAccess**的集合。</span><span class="sxs-lookup"><span data-stu-id="fddd3-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="fddd3-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fddd3-107">JSON representation</span></span>

<span data-ttu-id="fddd3-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fddd3-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="fddd3-109">属性</span><span class="sxs-lookup"><span data-stu-id="fddd3-109">Properties</span></span>
| <span data-ttu-id="fddd3-110">属性</span><span class="sxs-lookup"><span data-stu-id="fddd3-110">Property</span></span>     | <span data-ttu-id="fddd3-111">类型</span><span class="sxs-lookup"><span data-stu-id="fddd3-111">Type</span></span>   |<span data-ttu-id="fddd3-112">说明</span><span class="sxs-lookup"><span data-stu-id="fddd3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fddd3-113">id</span><span class="sxs-lookup"><span data-stu-id="fddd3-113">id</span></span>|<span data-ttu-id="fddd3-114">Guid</span><span class="sxs-lookup"><span data-stu-id="fddd3-114">Guid</span></span>|<span data-ttu-id="fddd3-115">资源应用程序公开的[oAuth2Permission](oauth2permission.md)或[appRole](approle.md)实例之一的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fddd3-115">The unique identifier for one of the [oAuth2Permission](oauth2permission.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="fddd3-116">type</span><span class="sxs-lookup"><span data-stu-id="fddd3-116">type</span></span>|<span data-ttu-id="fddd3-117">String</span><span class="sxs-lookup"><span data-stu-id="fddd3-117">String</span></span>|<span data-ttu-id="fddd3-118">指定**id**属性引用的是[oAuth2Permission](oauth2permission.md)还是[appRole](approle.md)。</span><span class="sxs-lookup"><span data-stu-id="fddd3-118">Specifies whether the **id** property references an [oAuth2Permission](oauth2permission.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="fddd3-119">可能的值为 "scope" 或 "role"。</span><span class="sxs-lookup"><span data-stu-id="fddd3-119">Possible values are "scope" or "role".</span></span>|

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

---
title: resourceAccess 资源类型
description: 指定应用程序所需的 OAuth 2.0 权限范围或应用程序角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: ffc1dc7b6a5c76903245f71d0d562a743b37f4d1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43368209"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="ccdd5-103">resourceAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="ccdd5-103">resourceAccess resource type</span></span>

<span data-ttu-id="ccdd5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccdd5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ccdd5-105">指定应用程序所需的 OAuth 2.0 权限范围或应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="ccdd5-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="ccdd5-106">[RequiredResourceAccess](requiredresourceaccess.md)类型的**ResourceAccess**属性是**resourceAccess**的集合。</span><span class="sxs-lookup"><span data-stu-id="ccdd5-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ccdd5-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ccdd5-107">JSON representation</span></span>

<span data-ttu-id="ccdd5-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ccdd5-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="ccdd5-109">属性</span><span class="sxs-lookup"><span data-stu-id="ccdd5-109">Properties</span></span>
| <span data-ttu-id="ccdd5-110">属性</span><span class="sxs-lookup"><span data-stu-id="ccdd5-110">Property</span></span>     | <span data-ttu-id="ccdd5-111">类型</span><span class="sxs-lookup"><span data-stu-id="ccdd5-111">Type</span></span>   |<span data-ttu-id="ccdd5-112">说明</span><span class="sxs-lookup"><span data-stu-id="ccdd5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccdd5-113">id</span><span class="sxs-lookup"><span data-stu-id="ccdd5-113">id</span></span>|<span data-ttu-id="ccdd5-114">Guid</span><span class="sxs-lookup"><span data-stu-id="ccdd5-114">Guid</span></span>|<span data-ttu-id="ccdd5-115">资源应用程序公开的[oauth2PermissionScopes](permissionscope.md)或[appRole](approle.md)实例之一的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ccdd5-115">The unique identifier for one of the [oauth2PermissionScopes](permissionscope.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="ccdd5-116">type</span><span class="sxs-lookup"><span data-stu-id="ccdd5-116">type</span></span>|<span data-ttu-id="ccdd5-117">String</span><span class="sxs-lookup"><span data-stu-id="ccdd5-117">String</span></span>|<span data-ttu-id="ccdd5-118">指定**id**属性引用的是[oauth2PermissionScopes](permissionscope.md)还是[appRole](approle.md)。</span><span class="sxs-lookup"><span data-stu-id="ccdd5-118">Specifies whether the **id** property references an [oauth2PermissionScopes](permissionscope.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="ccdd5-119">可能的值为 "scope" 或 "role"。</span><span class="sxs-lookup"><span data-stu-id="ccdd5-119">Possible values are "scope" or "role".</span></span>|

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

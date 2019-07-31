---
title: preAuthorizedApplication 资源类型
description: 表示应用程序和请求的隐式同意权限。 要求管理员向应用程序提供许可。 preAuthorizedApplications 不要求用户同意请求的权限。 PreAuthorizedApplications 中列出的权限不需要用户同意。 但是, preAuthorizedApplications 中未列出的任何其他请求的权限都需要用户同意。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7adaf4fe960b762b12f6b2cc8607e64c9813712e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965813"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="a6b58-107">preAuthorizedApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6b58-107">preAuthorizedApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6b58-108">表示应用程序和请求的隐式同意权限。</span><span class="sxs-lookup"><span data-stu-id="a6b58-108">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="a6b58-109">要求管理员向应用程序提供许可。</span><span class="sxs-lookup"><span data-stu-id="a6b58-109">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="a6b58-110">preAuthorizedApplications 不要求用户同意请求的权限。</span><span class="sxs-lookup"><span data-stu-id="a6b58-110">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="a6b58-111">PreAuthorizedApplications 中列出的权限不需要用户同意。</span><span class="sxs-lookup"><span data-stu-id="a6b58-111">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="a6b58-112">但是, preAuthorizedApplications 中未列出的任何其他请求的权限都需要用户同意。</span><span class="sxs-lookup"><span data-stu-id="a6b58-112">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="a6b58-113">属性</span><span class="sxs-lookup"><span data-stu-id="a6b58-113">Properties</span></span>

| <span data-ttu-id="a6b58-114">属性</span><span class="sxs-lookup"><span data-stu-id="a6b58-114">Property</span></span> | <span data-ttu-id="a6b58-115">类型</span><span class="sxs-lookup"><span data-stu-id="a6b58-115">Type</span></span> | <span data-ttu-id="a6b58-116">说明</span><span class="sxs-lookup"><span data-stu-id="a6b58-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a6b58-117">appId</span><span class="sxs-lookup"><span data-stu-id="a6b58-117">appId</span></span>|<span data-ttu-id="a6b58-118">String</span><span class="sxs-lookup"><span data-stu-id="a6b58-118">String</span></span>| <span data-ttu-id="a6b58-119">应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a6b58-119">The unique identifier for the application.</span></span> |
|<span data-ttu-id="a6b58-120">permissionIds</span><span class="sxs-lookup"><span data-stu-id="a6b58-120">permissionIds</span></span>|<span data-ttu-id="a6b58-121">String collection</span><span class="sxs-lookup"><span data-stu-id="a6b58-121">String collection</span></span>| <span data-ttu-id="a6b58-122">应用程序所需的[publishedPermissionScope](permissionscope.md)或[appRole](approle.md)的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a6b58-122">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a6b58-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6b58-123">JSON representation</span></span>
<span data-ttu-id="a6b58-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6b58-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "permissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

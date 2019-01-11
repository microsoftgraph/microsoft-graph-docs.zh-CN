---
title: preAuthorizedApplication 资源类型
description: 表示应用程序和隐式同意请求的权限。 需要管理员可以提供了到应用程序的许可。 preAuthorizedApplications 不需要用户同意所请求的权限。 PreAuthorizedApplications 中列出的权限不需要用户同意。 但是，preAuthorizedApplications 中未列出任何其他请求的权限要求用户同意。
localization_priority: Normal
ms.openlocfilehash: fa26b8046b81db70300b8ff40abcbd2b84f3f0c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832793"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="086b8-107">preAuthorizedApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="086b8-107">preAuthorizedApplication resource type</span></span>

> <span data-ttu-id="086b8-108">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="086b8-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="086b8-109">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="086b8-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="086b8-110">表示应用程序和隐式同意请求的权限。</span><span class="sxs-lookup"><span data-stu-id="086b8-110">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="086b8-111">需要管理员可以提供了到应用程序的许可。</span><span class="sxs-lookup"><span data-stu-id="086b8-111">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="086b8-112">preAuthorizedApplications 不需要用户同意所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="086b8-112">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="086b8-113">PreAuthorizedApplications 中列出的权限不需要用户同意。</span><span class="sxs-lookup"><span data-stu-id="086b8-113">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="086b8-114">但是，preAuthorizedApplications 中未列出任何其他请求的权限要求用户同意。</span><span class="sxs-lookup"><span data-stu-id="086b8-114">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="086b8-115">属性</span><span class="sxs-lookup"><span data-stu-id="086b8-115">Properties</span></span>

| <span data-ttu-id="086b8-116">属性</span><span class="sxs-lookup"><span data-stu-id="086b8-116">Property</span></span> | <span data-ttu-id="086b8-117">类型</span><span class="sxs-lookup"><span data-stu-id="086b8-117">Type</span></span> | <span data-ttu-id="086b8-118">Description</span><span class="sxs-lookup"><span data-stu-id="086b8-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="086b8-119">appId</span><span class="sxs-lookup"><span data-stu-id="086b8-119">appId</span></span>|<span data-ttu-id="086b8-120">String</span><span class="sxs-lookup"><span data-stu-id="086b8-120">String</span></span>| <span data-ttu-id="086b8-121">应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="086b8-121">The unique identifier for the application.</span></span> |
|<span data-ttu-id="086b8-122">permissionIds</span><span class="sxs-lookup"><span data-stu-id="086b8-122">permissionIds</span></span>|<span data-ttu-id="086b8-123">String 集合</span><span class="sxs-lookup"><span data-stu-id="086b8-123">String collection</span></span>| <span data-ttu-id="086b8-124">需要[publishedPermissionScope](permissionscope.md)或[appRole](approle.md)应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="086b8-124">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="086b8-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="086b8-125">JSON representation</span></span>
<span data-ttu-id="086b8-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="086b8-126">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

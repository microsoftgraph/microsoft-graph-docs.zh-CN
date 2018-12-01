---
title: preAuthorizedApplication 资源类型
description: 表示应用程序和隐式同意请求的权限。 需要管理员可以提供了到应用程序的许可。 preAuthorizedApplications 不需要用户同意所请求的权限。 PreAuthorizedApplications 中列出的权限不需要用户同意。 但是，preAuthorizedApplications 中未列出任何其他请求的权限要求用户同意。
ms.openlocfilehash: d299aefcac541407e0e42d0b0933e903afa3e84d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049092"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="e50f0-107">preAuthorizedApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="e50f0-107">preAuthorizedApplication resource type</span></span>

> <span data-ttu-id="e50f0-108">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e50f0-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e50f0-109">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e50f0-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e50f0-110">表示应用程序和隐式同意请求的权限。</span><span class="sxs-lookup"><span data-stu-id="e50f0-110">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="e50f0-111">需要管理员可以提供了到应用程序的许可。</span><span class="sxs-lookup"><span data-stu-id="e50f0-111">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="e50f0-112">preAuthorizedApplications 不需要用户同意所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="e50f0-112">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="e50f0-113">PreAuthorizedApplications 中列出的权限不需要用户同意。</span><span class="sxs-lookup"><span data-stu-id="e50f0-113">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="e50f0-114">但是，preAuthorizedApplications 中未列出任何其他请求的权限要求用户同意。</span><span class="sxs-lookup"><span data-stu-id="e50f0-114">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="e50f0-115">属性</span><span class="sxs-lookup"><span data-stu-id="e50f0-115">Properties</span></span>

| <span data-ttu-id="e50f0-116">属性</span><span class="sxs-lookup"><span data-stu-id="e50f0-116">Property</span></span> | <span data-ttu-id="e50f0-117">类型</span><span class="sxs-lookup"><span data-stu-id="e50f0-117">Type</span></span> | <span data-ttu-id="e50f0-118">说明</span><span class="sxs-lookup"><span data-stu-id="e50f0-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e50f0-119">appId</span><span class="sxs-lookup"><span data-stu-id="e50f0-119">appId</span></span>|<span data-ttu-id="e50f0-120">String</span><span class="sxs-lookup"><span data-stu-id="e50f0-120">String</span></span>| <span data-ttu-id="e50f0-121">应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e50f0-121">The unique identifier for the application.</span></span> |
|<span data-ttu-id="e50f0-122">permissionIds</span><span class="sxs-lookup"><span data-stu-id="e50f0-122">permissionIds</span></span>|<span data-ttu-id="e50f0-123">String 集合</span><span class="sxs-lookup"><span data-stu-id="e50f0-123">String collection</span></span>| <span data-ttu-id="e50f0-124">需要[publishedPermissionScope](permissionscope.md)或[appRole](approle.md)应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e50f0-124">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e50f0-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e50f0-125">JSON representation</span></span>
<span data-ttu-id="e50f0-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e50f0-126">Here is a JSON representation of the resource.</span></span>

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
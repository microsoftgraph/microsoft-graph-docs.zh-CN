---
author: rgregg
ms.author: rgregg
ms.date: 09/14/2017
title: 标识
localization_priority: Normal
ms.openlocfilehash: c1cd28f4c2932e4196605c408470948e5b570894
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847584"
---
# <a name="identity-resource-type"></a><span data-ttu-id="9b531-102">标识资源类型</span><span class="sxs-lookup"><span data-stu-id="9b531-102">identity resource type</span></span>

> <span data-ttu-id="9b531-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9b531-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b531-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9b531-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b531-p102">**身份**资源表示_主角_的身份。例如，主角可以是用户、设备或应用程序。</span><span class="sxs-lookup"><span data-stu-id="9b531-p102">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b531-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b531-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="9b531-108">属性</span><span class="sxs-lookup"><span data-stu-id="9b531-108">Properties</span></span>

| <span data-ttu-id="9b531-109">属性</span><span class="sxs-lookup"><span data-stu-id="9b531-109">Property</span></span>            | <span data-ttu-id="9b531-110">类型</span><span class="sxs-lookup"><span data-stu-id="9b531-110">Type</span></span>   | <span data-ttu-id="9b531-111">说明</span><span class="sxs-lookup"><span data-stu-id="9b531-111">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9b531-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9b531-112">displayName</span></span>         | <span data-ttu-id="9b531-113">字符串</span><span class="sxs-lookup"><span data-stu-id="9b531-113">String</span></span> | <span data-ttu-id="9b531-p103">此身份的显示名称。请注意，此信息不一定可查看或是最新的。例如，如果用户更改了其显示名称，API 可能会在以后的响应中显示新值，但与用户相关联的项在使用 [delta](../api/driveitem-delta.md) 时不会显示更改后的值。</span><span class="sxs-lookup"><span data-stu-id="9b531-p103">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>  |
| <span data-ttu-id="9b531-117">id</span><span class="sxs-lookup"><span data-stu-id="9b531-117">id</span></span>                  | <span data-ttu-id="9b531-118">String</span><span class="sxs-lookup"><span data-stu-id="9b531-118">String</span></span> | <span data-ttu-id="9b531-119">身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9b531-119">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="9b531-120">tenantId</span><span class="sxs-lookup"><span data-stu-id="9b531-120">tenantId</span></span>            | <span data-ttu-id="9b531-121">字符串</span><span class="sxs-lookup"><span data-stu-id="9b531-121">String</span></span> | <span data-ttu-id="9b531-122">（可选） 的租户的唯一标识。</span><span class="sxs-lookup"><span data-stu-id="9b531-122">Unique identity of the tenant (optional).</span></span>                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a><span data-ttu-id="9b531-123">注解</span><span class="sxs-lookup"><span data-stu-id="9b531-123">Remarks</span></span>

<span data-ttu-id="9b531-p104">在某些情况下，角色唯一标识符可能不可用。在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。</span><span class="sxs-lookup"><span data-stu-id="9b531-p104">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity"
} -->

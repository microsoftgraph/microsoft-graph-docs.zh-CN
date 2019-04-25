---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 身份
localization_priority: Normal
ms.openlocfilehash: 103657764b2f7073d553a01cd3794c0abecdf4f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567814"
---
# <a name="identity-resource-type"></a><span data-ttu-id="c4b46-102">Identity 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4b46-102">Identity resource type</span></span>

<span data-ttu-id="c4b46-p101">**身份**资源表示_主角_的身份。例如，主角可以是用户、设备或应用程序。</span><span class="sxs-lookup"><span data-stu-id="c4b46-p101">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4b46-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4b46-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity",
  "openType": true,
 "optionalProperties": ["displayName", "thumbnails"] } -->
```json
{
  "displayName": "string",
  "id": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="c4b46-106">属性</span><span class="sxs-lookup"><span data-stu-id="c4b46-106">Properties</span></span>

| <span data-ttu-id="c4b46-107">属性</span><span class="sxs-lookup"><span data-stu-id="c4b46-107">Property</span></span>    | <span data-ttu-id="c4b46-108">类型</span><span class="sxs-lookup"><span data-stu-id="c4b46-108">Type</span></span>   | <span data-ttu-id="c4b46-109">说明</span><span class="sxs-lookup"><span data-stu-id="c4b46-109">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c4b46-110">displayName</span><span class="sxs-lookup"><span data-stu-id="c4b46-110">displayName</span></span> | <span data-ttu-id="c4b46-111">String</span><span class="sxs-lookup"><span data-stu-id="c4b46-111">String</span></span> | <span data-ttu-id="c4b46-p102">此身份的显示名称。请注意，此信息不一定可查看或是最新的。例如，如果用户更改了其显示名称，API 可能会在以后的响应中显示新值，但与用户相关联的项在使用 [delta](../api/driveitem-delta.md) 时不会显示更改后的值。</span><span class="sxs-lookup"><span data-stu-id="c4b46-p102">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>     |
| <span data-ttu-id="c4b46-115">id</span><span class="sxs-lookup"><span data-stu-id="c4b46-115">id</span></span>          | <span data-ttu-id="c4b46-116">String</span><span class="sxs-lookup"><span data-stu-id="c4b46-116">String</span></span> | <span data-ttu-id="c4b46-117">身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c4b46-117">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |

## <a name="remarks"></a><span data-ttu-id="c4b46-118">注解</span><span class="sxs-lookup"><span data-stu-id="c4b46-118">Remarks</span></span>

<span data-ttu-id="c4b46-p103">在某些情况下，角色唯一标识符可能不可用。在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。</span><span class="sxs-lookup"><span data-stu-id="c4b46-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity"

} -->

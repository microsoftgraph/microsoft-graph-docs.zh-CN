---
title: targetResourceUser 资源类型
description: 指示已添加、 更新或删除管理员审核活动的一部分的用户对象。 派生 targetResource 资源。
ms.openlocfilehash: 632d0551b3aba434c3309c8c874947708eb9a9f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044761"
---
# <a name="targetresourceuser-resource-type"></a><span data-ttu-id="bc7ed-104">targetResourceUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc7ed-104">targetResourceUser resource type</span></span>
<span data-ttu-id="bc7ed-105">指示已添加、 更新或删除管理员审核活动的一部分的用户对象。</span><span class="sxs-lookup"><span data-stu-id="bc7ed-105">Indicates the user object that was added, updated or deleted by admins as part of audit activity.</span></span> <span data-ttu-id="bc7ed-106">派生[targetResource](targetresource.md)资源。</span><span class="sxs-lookup"><span data-stu-id="bc7ed-106">Derived from the [targetResource](targetresource.md) resource.</span></span>


## <a name="properties"></a><span data-ttu-id="bc7ed-107">属性</span><span class="sxs-lookup"><span data-stu-id="bc7ed-107">Properties</span></span>
| <span data-ttu-id="bc7ed-108">属性</span><span class="sxs-lookup"><span data-stu-id="bc7ed-108">Property</span></span>     | <span data-ttu-id="bc7ed-109">类型</span><span class="sxs-lookup"><span data-stu-id="bc7ed-109">Type</span></span>   |<span data-ttu-id="bc7ed-110">说明</span><span class="sxs-lookup"><span data-stu-id="bc7ed-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc7ed-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bc7ed-111">userPrincipalName</span></span>|<span data-ttu-id="bc7ed-112">字符串</span><span class="sxs-lookup"><span data-stu-id="bc7ed-112">String</span></span>|<span data-ttu-id="bc7ed-113">指示用户的唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="bc7ed-113">Indicates the Unique Id of the User.</span></span> <span data-ttu-id="bc7ed-114">为某个特定用户是指用户 Id。</span><span class="sxs-lookup"><span data-stu-id="bc7ed-114">Refers to User Id for a specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc7ed-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc7ed-115">JSON representation</span></span>

<span data-ttu-id="bc7ed-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc7ed-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceUser"
}-->

```json
{
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
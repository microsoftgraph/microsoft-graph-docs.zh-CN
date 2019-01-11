---
title: targetResourceUser 资源类型
description: 指示已添加、 更新或删除管理员审核活动的一部分的用户对象。 派生 targetResource 资源。
localization_priority: Normal
ms.openlocfilehash: 9c71ead1b358b72a1b531abac56018fa71d084e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831926"
---
# <a name="targetresourceuser-resource-type"></a><span data-ttu-id="1d48c-104">targetResourceUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d48c-104">targetResourceUser resource type</span></span>
<span data-ttu-id="1d48c-105">指示已添加、 更新或删除管理员审核活动的一部分的用户对象。</span><span class="sxs-lookup"><span data-stu-id="1d48c-105">Indicates the user object that was added, updated or deleted by admins as part of audit activity.</span></span> <span data-ttu-id="1d48c-106">派生[targetResource](targetresource.md)资源。</span><span class="sxs-lookup"><span data-stu-id="1d48c-106">Derived from the [targetResource](targetresource.md) resource.</span></span>


## <a name="properties"></a><span data-ttu-id="1d48c-107">属性</span><span class="sxs-lookup"><span data-stu-id="1d48c-107">Properties</span></span>
| <span data-ttu-id="1d48c-108">属性</span><span class="sxs-lookup"><span data-stu-id="1d48c-108">Property</span></span>     | <span data-ttu-id="1d48c-109">类型</span><span class="sxs-lookup"><span data-stu-id="1d48c-109">Type</span></span>   |<span data-ttu-id="1d48c-110">说明</span><span class="sxs-lookup"><span data-stu-id="1d48c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d48c-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1d48c-111">userPrincipalName</span></span>|<span data-ttu-id="1d48c-112">字符串</span><span class="sxs-lookup"><span data-stu-id="1d48c-112">String</span></span>|<span data-ttu-id="1d48c-113">指示用户的唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="1d48c-113">Indicates the Unique Id of the User.</span></span> <span data-ttu-id="1d48c-114">为某个特定用户是指用户 Id。</span><span class="sxs-lookup"><span data-stu-id="1d48c-114">Refers to User Id for a specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d48c-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d48c-115">JSON representation</span></span>

<span data-ttu-id="1d48c-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d48c-116">Here is a JSON representation of the resource.</span></span>

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

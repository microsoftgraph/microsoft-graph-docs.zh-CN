---
title: governanceSubject 资源类型
description: 表示在特权标识管理 (PIM) 中管理的用户、组和服务主体。
localization_priority: Normal
ms.openlocfilehash: 5ad4b30abaec66b8ad35835795848645ddd9f17b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333684"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="032ab-103">governanceSubject 资源类型</span><span class="sxs-lookup"><span data-stu-id="032ab-103">governanceSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="032ab-104">表示在特权标识管理 (PIM) 中管理的用户、组和服务主体。</span><span class="sxs-lookup"><span data-stu-id="032ab-104">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="032ab-105">属性</span><span class="sxs-lookup"><span data-stu-id="032ab-105">Properties</span></span>
| <span data-ttu-id="032ab-106">属性</span><span class="sxs-lookup"><span data-stu-id="032ab-106">Property</span></span>  | <span data-ttu-id="032ab-107">类型</span><span class="sxs-lookup"><span data-stu-id="032ab-107">Type</span></span>       |<span data-ttu-id="032ab-108">说明</span><span class="sxs-lookup"><span data-stu-id="032ab-108">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="032ab-109">id</span><span class="sxs-lookup"><span data-stu-id="032ab-109">id</span></span>         |<span data-ttu-id="032ab-110">String</span><span class="sxs-lookup"><span data-stu-id="032ab-110">String</span></span>     | <span data-ttu-id="032ab-111">主题的 id。</span><span class="sxs-lookup"><span data-stu-id="032ab-111">The id of the subject.</span></span>|
|<span data-ttu-id="032ab-112">type</span><span class="sxs-lookup"><span data-stu-id="032ab-112">type</span></span>       |<span data-ttu-id="032ab-113">String</span><span class="sxs-lookup"><span data-stu-id="032ab-113">String</span></span>     |<span data-ttu-id="032ab-114">主题的类型。</span><span class="sxs-lookup"><span data-stu-id="032ab-114">The type of the subject.</span></span> <span data-ttu-id="032ab-115">值可以是``User``、 ``Group``和。 ``ServicePrincipal``</span><span class="sxs-lookup"><span data-stu-id="032ab-115">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="032ab-116">displayName</span><span class="sxs-lookup"><span data-stu-id="032ab-116">displayName</span></span>|<span data-ttu-id="032ab-117">String</span><span class="sxs-lookup"><span data-stu-id="032ab-117">String</span></span>     |<span data-ttu-id="032ab-118">主题的显示名称。</span><span class="sxs-lookup"><span data-stu-id="032ab-118">The display name of the subject.</span></span>|
|<span data-ttu-id="032ab-119">email</span><span class="sxs-lookup"><span data-stu-id="032ab-119">email</span></span>      |<span data-ttu-id="032ab-120">字符串</span><span class="sxs-lookup"><span data-stu-id="032ab-120">String</span></span>     |<span data-ttu-id="032ab-121">用户主题的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="032ab-121">The email address of the user subject.</span></span> <span data-ttu-id="032ab-122">如果主题在其他类型中, 则为空。</span><span class="sxs-lookup"><span data-stu-id="032ab-122">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="032ab-123">principalName</span><span class="sxs-lookup"><span data-stu-id="032ab-123">principalName</span></span>|<span data-ttu-id="032ab-124">String</span><span class="sxs-lookup"><span data-stu-id="032ab-124">String</span></span>   |<span data-ttu-id="032ab-125">用户主题的主体名称。</span><span class="sxs-lookup"><span data-stu-id="032ab-125">The principal name of the user subject.</span></span> <span data-ttu-id="032ab-126">如果主题在其他类型中, 则为空。</span><span class="sxs-lookup"><span data-stu-id="032ab-126">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="032ab-127">关系</span><span class="sxs-lookup"><span data-stu-id="032ab-127">Relationships</span></span>
<span data-ttu-id="032ab-128">无</span><span class="sxs-lookup"><span data-stu-id="032ab-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="032ab-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="032ab-129">JSON representation</span></span>

<span data-ttu-id="032ab-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="032ab-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSubject"
}-->

```json
{
  "id": "String",  
  "displayName": "String",
  "email": "String",
  "principalName": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

---
title: governanceSubject 资源类型
description: 表示在特权身份管理 (PIM) 中管理的用户、组和服务主体。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 384558109521fe93c5ef4331e88355c8757cf5fc
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809486"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="30a15-103">governanceSubject 资源类型</span><span class="sxs-lookup"><span data-stu-id="30a15-103">governanceSubject resource type</span></span>

<span data-ttu-id="30a15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30a15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30a15-105">表示在特权身份管理 (PIM) 中管理的用户、组和服务主体。</span><span class="sxs-lookup"><span data-stu-id="30a15-105">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="30a15-106">属性</span><span class="sxs-lookup"><span data-stu-id="30a15-106">Properties</span></span>
| <span data-ttu-id="30a15-107">属性</span><span class="sxs-lookup"><span data-stu-id="30a15-107">Property</span></span>  | <span data-ttu-id="30a15-108">类型</span><span class="sxs-lookup"><span data-stu-id="30a15-108">Type</span></span>       |<span data-ttu-id="30a15-109">说明</span><span class="sxs-lookup"><span data-stu-id="30a15-109">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="30a15-110">id</span><span class="sxs-lookup"><span data-stu-id="30a15-110">id</span></span>         |<span data-ttu-id="30a15-111">String</span><span class="sxs-lookup"><span data-stu-id="30a15-111">String</span></span>     | <span data-ttu-id="30a15-112">主题的 id。</span><span class="sxs-lookup"><span data-stu-id="30a15-112">The id of the subject.</span></span>|
|<span data-ttu-id="30a15-113">type</span><span class="sxs-lookup"><span data-stu-id="30a15-113">type</span></span>       |<span data-ttu-id="30a15-114">String</span><span class="sxs-lookup"><span data-stu-id="30a15-114">String</span></span>     |<span data-ttu-id="30a15-115">主题的类型。</span><span class="sxs-lookup"><span data-stu-id="30a15-115">The type of the subject.</span></span> <span data-ttu-id="30a15-116">值可以是 ``User`` 、 ``Group`` 和 ``ServicePrincipal`` 。</span><span class="sxs-lookup"><span data-stu-id="30a15-116">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="30a15-117">displayName</span><span class="sxs-lookup"><span data-stu-id="30a15-117">displayName</span></span>|<span data-ttu-id="30a15-118">String</span><span class="sxs-lookup"><span data-stu-id="30a15-118">String</span></span>     |<span data-ttu-id="30a15-119">主题的显示名称。</span><span class="sxs-lookup"><span data-stu-id="30a15-119">The display name of the subject.</span></span>|
|<span data-ttu-id="30a15-120">email</span><span class="sxs-lookup"><span data-stu-id="30a15-120">email</span></span>      |<span data-ttu-id="30a15-121">String</span><span class="sxs-lookup"><span data-stu-id="30a15-121">String</span></span>     |<span data-ttu-id="30a15-122">用户主题的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="30a15-122">The email address of the user subject.</span></span> <span data-ttu-id="30a15-123">如果主题在其他类型中，则为空。</span><span class="sxs-lookup"><span data-stu-id="30a15-123">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="30a15-124">principalName</span><span class="sxs-lookup"><span data-stu-id="30a15-124">principalName</span></span>|<span data-ttu-id="30a15-125">String</span><span class="sxs-lookup"><span data-stu-id="30a15-125">String</span></span>   |<span data-ttu-id="30a15-126">用户主题的主体名称。</span><span class="sxs-lookup"><span data-stu-id="30a15-126">The principal name of the user subject.</span></span> <span data-ttu-id="30a15-127">如果主题在其他类型中，则为空。</span><span class="sxs-lookup"><span data-stu-id="30a15-127">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30a15-128">关系</span><span class="sxs-lookup"><span data-stu-id="30a15-128">Relationships</span></span>
<span data-ttu-id="30a15-129">无</span><span class="sxs-lookup"><span data-stu-id="30a15-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="30a15-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30a15-130">JSON representation</span></span>

<span data-ttu-id="30a15-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30a15-131">Here is a JSON representation of the resource.</span></span>

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

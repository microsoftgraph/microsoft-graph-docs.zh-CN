---
title: governanceSubject 资源类型
description: 表示在 PRIVILEGEd Identity Management 中管理的用户、组和服务主体 (PIM) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: eedcaff8538d5a0efa110b34cd6a72aef2a3210a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132671"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="a9802-103">governanceSubject 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9802-103">governanceSubject resource type</span></span>

<span data-ttu-id="a9802-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9802-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9802-105">表示在 PRIVILEGEd Identity Management 中管理的用户、组和服务主体 (PIM) 。</span><span class="sxs-lookup"><span data-stu-id="a9802-105">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="a9802-106">属性</span><span class="sxs-lookup"><span data-stu-id="a9802-106">Properties</span></span>
| <span data-ttu-id="a9802-107">属性</span><span class="sxs-lookup"><span data-stu-id="a9802-107">Property</span></span>  | <span data-ttu-id="a9802-108">类型</span><span class="sxs-lookup"><span data-stu-id="a9802-108">Type</span></span>       |<span data-ttu-id="a9802-109">说明</span><span class="sxs-lookup"><span data-stu-id="a9802-109">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="a9802-110">id</span><span class="sxs-lookup"><span data-stu-id="a9802-110">id</span></span>         |<span data-ttu-id="a9802-111">字符串</span><span class="sxs-lookup"><span data-stu-id="a9802-111">String</span></span>     | <span data-ttu-id="a9802-112">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="a9802-112">The id of the subject.</span></span>|
|<span data-ttu-id="a9802-113">type</span><span class="sxs-lookup"><span data-stu-id="a9802-113">type</span></span>       |<span data-ttu-id="a9802-114">字符串</span><span class="sxs-lookup"><span data-stu-id="a9802-114">String</span></span>     |<span data-ttu-id="a9802-115">主题的类型。</span><span class="sxs-lookup"><span data-stu-id="a9802-115">The type of the subject.</span></span> <span data-ttu-id="a9802-116">值可以是 ``User`` 、 ``Group`` 和 ``ServicePrincipal`` 。</span><span class="sxs-lookup"><span data-stu-id="a9802-116">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="a9802-117">displayName</span><span class="sxs-lookup"><span data-stu-id="a9802-117">displayName</span></span>|<span data-ttu-id="a9802-118">字符串</span><span class="sxs-lookup"><span data-stu-id="a9802-118">String</span></span>     |<span data-ttu-id="a9802-119">主题显示名称。</span><span class="sxs-lookup"><span data-stu-id="a9802-119">The display name of the subject.</span></span>|
|<span data-ttu-id="a9802-120">email</span><span class="sxs-lookup"><span data-stu-id="a9802-120">email</span></span>      |<span data-ttu-id="a9802-121">字符串</span><span class="sxs-lookup"><span data-stu-id="a9802-121">String</span></span>     |<span data-ttu-id="a9802-122">用户主题的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a9802-122">The email address of the user subject.</span></span> <span data-ttu-id="a9802-123">如果主题为其他类型的主题，则为空。</span><span class="sxs-lookup"><span data-stu-id="a9802-123">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="a9802-124">principalName</span><span class="sxs-lookup"><span data-stu-id="a9802-124">principalName</span></span>|<span data-ttu-id="a9802-125">String</span><span class="sxs-lookup"><span data-stu-id="a9802-125">String</span></span>   |<span data-ttu-id="a9802-126">用户主题的主体名称。</span><span class="sxs-lookup"><span data-stu-id="a9802-126">The principal name of the user subject.</span></span> <span data-ttu-id="a9802-127">如果主题为其他类型的主题，则为空。</span><span class="sxs-lookup"><span data-stu-id="a9802-127">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9802-128">关系</span><span class="sxs-lookup"><span data-stu-id="a9802-128">Relationships</span></span>
<span data-ttu-id="a9802-129">无</span><span class="sxs-lookup"><span data-stu-id="a9802-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a9802-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9802-130">JSON representation</span></span>

<span data-ttu-id="a9802-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9802-131">Here is a JSON representation of the resource.</span></span>

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



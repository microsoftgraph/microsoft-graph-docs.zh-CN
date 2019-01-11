---
title: governanceSubject 资源类型
description: 表示用户、 组和管理特权标识管理 (PIM) 中的服务主体。
localization_priority: Normal
ms.openlocfilehash: f3f8762c9136a3ae92269f6c06f52000fb73f710
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832589"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="73334-103">governanceSubject 资源类型</span><span class="sxs-lookup"><span data-stu-id="73334-103">governanceSubject resource type</span></span>

> <span data-ttu-id="73334-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="73334-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73334-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="73334-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73334-106">表示用户、 组和管理特权标识管理 (PIM) 中的服务主体。</span><span class="sxs-lookup"><span data-stu-id="73334-106">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="73334-107">属性</span><span class="sxs-lookup"><span data-stu-id="73334-107">Properties</span></span>
| <span data-ttu-id="73334-108">属性</span><span class="sxs-lookup"><span data-stu-id="73334-108">Property</span></span>  | <span data-ttu-id="73334-109">类型</span><span class="sxs-lookup"><span data-stu-id="73334-109">Type</span></span>       |<span data-ttu-id="73334-110">说明</span><span class="sxs-lookup"><span data-stu-id="73334-110">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="73334-111">id</span><span class="sxs-lookup"><span data-stu-id="73334-111">id</span></span>         |<span data-ttu-id="73334-112">字符串</span><span class="sxs-lookup"><span data-stu-id="73334-112">String</span></span>     | <span data-ttu-id="73334-113">主题的 id。</span><span class="sxs-lookup"><span data-stu-id="73334-113">The id of the subject.</span></span>|
|<span data-ttu-id="73334-114">type</span><span class="sxs-lookup"><span data-stu-id="73334-114">type</span></span>       |<span data-ttu-id="73334-115">字符串</span><span class="sxs-lookup"><span data-stu-id="73334-115">String</span></span>     |<span data-ttu-id="73334-116">主题类型。</span><span class="sxs-lookup"><span data-stu-id="73334-116">The type of the subject.</span></span> <span data-ttu-id="73334-117">值可以是``User``， ``Group``，和``ServicePrincipal``。</span><span class="sxs-lookup"><span data-stu-id="73334-117">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="73334-118">displayName</span><span class="sxs-lookup"><span data-stu-id="73334-118">displayName</span></span>|<span data-ttu-id="73334-119">字符串</span><span class="sxs-lookup"><span data-stu-id="73334-119">String</span></span>     |<span data-ttu-id="73334-120">主题的显示名称。</span><span class="sxs-lookup"><span data-stu-id="73334-120">The display name of the subject.</span></span>|
|<span data-ttu-id="73334-121">email</span><span class="sxs-lookup"><span data-stu-id="73334-121">email</span></span>      |<span data-ttu-id="73334-122">字符串</span><span class="sxs-lookup"><span data-stu-id="73334-122">String</span></span>     |<span data-ttu-id="73334-123">用户使用者的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="73334-123">The email address of the user subject.</span></span> <span data-ttu-id="73334-124">如果主题位于其他类型，它为空。</span><span class="sxs-lookup"><span data-stu-id="73334-124">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="73334-125">principalName</span><span class="sxs-lookup"><span data-stu-id="73334-125">principalName</span></span>|<span data-ttu-id="73334-126">String</span><span class="sxs-lookup"><span data-stu-id="73334-126">String</span></span>   |<span data-ttu-id="73334-127">主体的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="73334-127">The principal name of the user subject.</span></span> <span data-ttu-id="73334-128">如果主题位于其他类型，它为空。</span><span class="sxs-lookup"><span data-stu-id="73334-128">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73334-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="73334-129">Relationships</span></span>
<span data-ttu-id="73334-130">无</span><span class="sxs-lookup"><span data-stu-id="73334-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="73334-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73334-131">JSON representation</span></span>

<span data-ttu-id="73334-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73334-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

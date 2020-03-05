---
title: profilePhoto 资源类型
description: 从 Exchange Online 访问的用户、组或 Outlook 联系人的个人资料照片。它是不以 base-64 编码的二进制数据。
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3420f229d26ecbcce1a39de03c50dd084c828d94
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447057"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="cee73-104">profilePhoto 资源类型</span><span class="sxs-lookup"><span data-stu-id="cee73-104">profilePhoto resource type</span></span>

<span data-ttu-id="cee73-p102">命名空间：microsoft.graph 从 Exchange Online 访问的用户、组或 Outlook 联系人的个人资料照片。它是不以 base-64 编码的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="cee73-p102">Namespace: microsoft.graph A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="cee73-107">Exchange Online 支持的 HD 照片大小如下所示：'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504' 和 '648x648'。</span><span class="sxs-lookup"><span data-stu-id="cee73-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="cee73-108">方法</span><span class="sxs-lookup"><span data-stu-id="cee73-108">Methods</span></span>

| <span data-ttu-id="cee73-109">方法</span><span class="sxs-lookup"><span data-stu-id="cee73-109">Method</span></span>       | <span data-ttu-id="cee73-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cee73-110">Return Type</span></span>  |<span data-ttu-id="cee73-111">说明</span><span class="sxs-lookup"><span data-stu-id="cee73-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cee73-112">获取 profilePhoto</span><span class="sxs-lookup"><span data-stu-id="cee73-112">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="cee73-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="cee73-113">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="cee73-114">获取指定的 **profilePhoto** 或其元数据（profilePhoto 属性）。</span><span class="sxs-lookup"><span data-stu-id="cee73-114">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="cee73-115">更新</span><span class="sxs-lookup"><span data-stu-id="cee73-115">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="cee73-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="cee73-116">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="cee73-p103">将照片分配给指定的用户、组或联系人。照片应为二进制格式。它将替换现有的照片（如有）。</span><span class="sxs-lookup"><span data-stu-id="cee73-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="cee73-120">属性</span><span class="sxs-lookup"><span data-stu-id="cee73-120">Properties</span></span>
| <span data-ttu-id="cee73-121">属性</span><span class="sxs-lookup"><span data-stu-id="cee73-121">Property</span></span>     | <span data-ttu-id="cee73-122">类型</span><span class="sxs-lookup"><span data-stu-id="cee73-122">Type</span></span>   |<span data-ttu-id="cee73-123">说明</span><span class="sxs-lookup"><span data-stu-id="cee73-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cee73-124">id</span><span class="sxs-lookup"><span data-stu-id="cee73-124">id</span></span>|<span data-ttu-id="cee73-125">string</span><span class="sxs-lookup"><span data-stu-id="cee73-125">string</span></span>|<span data-ttu-id="cee73-126">只读。</span><span class="sxs-lookup"><span data-stu-id="cee73-126">Read-only.</span></span>|
|<span data-ttu-id="cee73-127">height</span><span class="sxs-lookup"><span data-stu-id="cee73-127">height</span></span>|<span data-ttu-id="cee73-128">int32</span><span class="sxs-lookup"><span data-stu-id="cee73-128">int32</span></span>|<span data-ttu-id="cee73-p104">照片的高度。只读。</span><span class="sxs-lookup"><span data-stu-id="cee73-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="cee73-131">width</span><span class="sxs-lookup"><span data-stu-id="cee73-131">width</span></span>|<span data-ttu-id="cee73-132">int32</span><span class="sxs-lookup"><span data-stu-id="cee73-132">int32</span></span>|<span data-ttu-id="cee73-p105">照片的宽度。只读。</span><span class="sxs-lookup"><span data-stu-id="cee73-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cee73-135">关系</span><span class="sxs-lookup"><span data-stu-id="cee73-135">Relationships</span></span>
<span data-ttu-id="cee73-136">无</span><span class="sxs-lookup"><span data-stu-id="cee73-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cee73-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cee73-137">JSON representation</span></span>

<span data-ttu-id="cee73-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cee73-138">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "isMediaEntity": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

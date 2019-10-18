---
title: profilePhoto 资源类型
description: 从 Exchange Online 访问的用户、组或 Outlook 联系人的个人资料照片。它是不以 base-64 编码的二进制数据。
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: baee7eebd3abcaa8376440fb0b20cbe5c69df880
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035054"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="d7cb9-104">profilePhoto 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7cb9-104">profilePhoto resource type</span></span>
<span data-ttu-id="d7cb9-p102">从 Exchange Online 访问的用户、组或 Outlook 联系人的个人资料照片。它是不以 base-64 编码的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="d7cb9-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="d7cb9-107">Exchange Online 支持的 HD 照片大小如下所示：'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504' 和 '648x648'。</span><span class="sxs-lookup"><span data-stu-id="d7cb9-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="d7cb9-108">方法</span><span class="sxs-lookup"><span data-stu-id="d7cb9-108">Methods</span></span>

| <span data-ttu-id="d7cb9-109">方法</span><span class="sxs-lookup"><span data-stu-id="d7cb9-109">Method</span></span>       | <span data-ttu-id="d7cb9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d7cb9-110">Return Type</span></span>  |<span data-ttu-id="d7cb9-111">说明</span><span class="sxs-lookup"><span data-stu-id="d7cb9-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d7cb9-112">获取 profilePhoto</span><span class="sxs-lookup"><span data-stu-id="d7cb9-112">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="d7cb9-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="d7cb9-113">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="d7cb9-114">获取指定的 **profilePhoto** 或其元数据（profilePhoto 属性）。</span><span class="sxs-lookup"><span data-stu-id="d7cb9-114">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="d7cb9-115">更新</span><span class="sxs-lookup"><span data-stu-id="d7cb9-115">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="d7cb9-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="d7cb9-116">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="d7cb9-p103">将照片分配给指定的用户、组或联系人。照片应为二进制格式。它将替换现有的照片（如有）。</span><span class="sxs-lookup"><span data-stu-id="d7cb9-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="d7cb9-120">属性</span><span class="sxs-lookup"><span data-stu-id="d7cb9-120">Properties</span></span>
| <span data-ttu-id="d7cb9-121">属性</span><span class="sxs-lookup"><span data-stu-id="d7cb9-121">Property</span></span>     | <span data-ttu-id="d7cb9-122">类型</span><span class="sxs-lookup"><span data-stu-id="d7cb9-122">Type</span></span>   |<span data-ttu-id="d7cb9-123">说明</span><span class="sxs-lookup"><span data-stu-id="d7cb9-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7cb9-124">id</span><span class="sxs-lookup"><span data-stu-id="d7cb9-124">id</span></span>|<span data-ttu-id="d7cb9-125">string</span><span class="sxs-lookup"><span data-stu-id="d7cb9-125">string</span></span>|<span data-ttu-id="d7cb9-126">只读。</span><span class="sxs-lookup"><span data-stu-id="d7cb9-126">Read-only.</span></span>|
|<span data-ttu-id="d7cb9-127">height</span><span class="sxs-lookup"><span data-stu-id="d7cb9-127">height</span></span>|<span data-ttu-id="d7cb9-128">int32</span><span class="sxs-lookup"><span data-stu-id="d7cb9-128">int32</span></span>|<span data-ttu-id="d7cb9-p104">照片的高度。只读。</span><span class="sxs-lookup"><span data-stu-id="d7cb9-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="d7cb9-131">width</span><span class="sxs-lookup"><span data-stu-id="d7cb9-131">width</span></span>|<span data-ttu-id="d7cb9-132">int32</span><span class="sxs-lookup"><span data-stu-id="d7cb9-132">int32</span></span>|<span data-ttu-id="d7cb9-p105">照片的宽度。只读。</span><span class="sxs-lookup"><span data-stu-id="d7cb9-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7cb9-135">关系</span><span class="sxs-lookup"><span data-stu-id="d7cb9-135">Relationships</span></span>
<span data-ttu-id="d7cb9-136">无</span><span class="sxs-lookup"><span data-stu-id="d7cb9-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d7cb9-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7cb9-137">JSON representation</span></span>

<span data-ttu-id="d7cb9-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7cb9-138">Here is a JSON representation of the resource.</span></span>

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

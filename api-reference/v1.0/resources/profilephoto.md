---
title: profilePhoto 资源类型
description: 从 Exchange Online 访问的用户、组或 Outlook 联系人的个人资料照片。它是不以 base-64 编码的二进制数据。
ms.openlocfilehash: c5f74e1dcd48e42a2e17d5a64e6ed4b9e9cca5e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011609"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="f638b-104">profilePhoto 资源类型</span><span class="sxs-lookup"><span data-stu-id="f638b-104">profilePhoto resource type</span></span>
<span data-ttu-id="f638b-p102">从 Exchange Online 访问的用户、组或 Outlook 联系人的个人资料照片。它是不以 base-64 编码的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="f638b-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="f638b-107">Exchange Online 支持的 HD 照片大小如下所示：'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504' 和 '648x648'。</span><span class="sxs-lookup"><span data-stu-id="f638b-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="f638b-108">方法</span><span class="sxs-lookup"><span data-stu-id="f638b-108">Methods</span></span>

| <span data-ttu-id="f638b-109">方法</span><span class="sxs-lookup"><span data-stu-id="f638b-109">Method</span></span>       | <span data-ttu-id="f638b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f638b-110">Return Type</span></span>  |<span data-ttu-id="f638b-111">说明</span><span class="sxs-lookup"><span data-stu-id="f638b-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f638b-112">获取 profilePhoto</span><span class="sxs-lookup"><span data-stu-id="f638b-112">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="f638b-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="f638b-113">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="f638b-114">获取指定的 **profilePhoto** 或其元数据（profilePhoto 属性）。</span><span class="sxs-lookup"><span data-stu-id="f638b-114">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="f638b-115">更新</span><span class="sxs-lookup"><span data-stu-id="f638b-115">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="f638b-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="f638b-116">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="f638b-p103">将照片分配给指定的用户、组或联系人。照片应为二进制格式。它将替换现有的照片（如有）。</span><span class="sxs-lookup"><span data-stu-id="f638b-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="f638b-120">属性</span><span class="sxs-lookup"><span data-stu-id="f638b-120">Properties</span></span>
| <span data-ttu-id="f638b-121">属性</span><span class="sxs-lookup"><span data-stu-id="f638b-121">Property</span></span>     | <span data-ttu-id="f638b-122">类型</span><span class="sxs-lookup"><span data-stu-id="f638b-122">Type</span></span>   |<span data-ttu-id="f638b-123">说明</span><span class="sxs-lookup"><span data-stu-id="f638b-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f638b-124">ID</span><span class="sxs-lookup"><span data-stu-id="f638b-124">id</span></span>|<span data-ttu-id="f638b-125">string</span><span class="sxs-lookup"><span data-stu-id="f638b-125">string</span></span>|<span data-ttu-id="f638b-126">只读。</span><span class="sxs-lookup"><span data-stu-id="f638b-126">Read-only.</span></span>|
|<span data-ttu-id="f638b-127">height</span><span class="sxs-lookup"><span data-stu-id="f638b-127">height</span></span>|<span data-ttu-id="f638b-128">int32</span><span class="sxs-lookup"><span data-stu-id="f638b-128">int32</span></span>|<span data-ttu-id="f638b-p104">照片的高度。只读。</span><span class="sxs-lookup"><span data-stu-id="f638b-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="f638b-131">width</span><span class="sxs-lookup"><span data-stu-id="f638b-131">width</span></span>|<span data-ttu-id="f638b-132">int32</span><span class="sxs-lookup"><span data-stu-id="f638b-132">int32</span></span>|<span data-ttu-id="f638b-p105">照片的宽度。只读。</span><span class="sxs-lookup"><span data-stu-id="f638b-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f638b-135">Relationships</span><span class="sxs-lookup"><span data-stu-id="f638b-135">Relationships</span></span>
<span data-ttu-id="f638b-136">无</span><span class="sxs-lookup"><span data-stu-id="f638b-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f638b-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f638b-137">JSON representation</span></span>

<span data-ttu-id="f638b-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f638b-138">Here is a JSON representation of the resource.</span></span>

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

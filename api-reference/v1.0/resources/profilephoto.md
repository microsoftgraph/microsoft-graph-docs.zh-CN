---
title: profilePhoto 资源类型
description: 从 Exchange Online 访问的用户、组或 Outlook 联系人的个人资料照片。它是不以 base-64 编码的二进制数据。
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d11d5043e759900810315d4b3e3af8310cb996f0
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934904"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="9022d-104">profilePhoto 资源类型</span><span class="sxs-lookup"><span data-stu-id="9022d-104">profilePhoto resource type</span></span>

<span data-ttu-id="9022d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9022d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9022d-p102">从 Exchange Online 访问的用户、组或 Outlook 联系人的个人资料照片。它是不以 base-64 编码的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="9022d-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="9022d-108">Exchange Online 支持的 HD 照片大小如下所示：'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504' 和 '648x648'。</span><span class="sxs-lookup"><span data-stu-id="9022d-108">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="9022d-109">方法</span><span class="sxs-lookup"><span data-stu-id="9022d-109">Methods</span></span>

| <span data-ttu-id="9022d-110">方法</span><span class="sxs-lookup"><span data-stu-id="9022d-110">Method</span></span>       | <span data-ttu-id="9022d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="9022d-111">Return Type</span></span>  |<span data-ttu-id="9022d-112">说明</span><span class="sxs-lookup"><span data-stu-id="9022d-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9022d-113">获取 profilePhoto</span><span class="sxs-lookup"><span data-stu-id="9022d-113">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="9022d-114">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="9022d-114">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="9022d-115">获取指定的 **profilePhoto** 或其元数据（profilePhoto 属性）。</span><span class="sxs-lookup"><span data-stu-id="9022d-115">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="9022d-116">更新</span><span class="sxs-lookup"><span data-stu-id="9022d-116">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="9022d-117">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="9022d-117">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="9022d-p103">将照片分配给指定的用户、组或联系人。照片应为二进制格式。它将替换现有的照片（如有）。</span><span class="sxs-lookup"><span data-stu-id="9022d-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="9022d-121">属性</span><span class="sxs-lookup"><span data-stu-id="9022d-121">Properties</span></span>
| <span data-ttu-id="9022d-122">属性</span><span class="sxs-lookup"><span data-stu-id="9022d-122">Property</span></span>     | <span data-ttu-id="9022d-123">类型</span><span class="sxs-lookup"><span data-stu-id="9022d-123">Type</span></span>   |<span data-ttu-id="9022d-124">说明</span><span class="sxs-lookup"><span data-stu-id="9022d-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9022d-125">id</span><span class="sxs-lookup"><span data-stu-id="9022d-125">id</span></span>|<span data-ttu-id="9022d-126">string</span><span class="sxs-lookup"><span data-stu-id="9022d-126">string</span></span>|<span data-ttu-id="9022d-127">只读。</span><span class="sxs-lookup"><span data-stu-id="9022d-127">Read-only.</span></span>|
|<span data-ttu-id="9022d-128">height</span><span class="sxs-lookup"><span data-stu-id="9022d-128">height</span></span>|<span data-ttu-id="9022d-129">int32</span><span class="sxs-lookup"><span data-stu-id="9022d-129">int32</span></span>|<span data-ttu-id="9022d-p104">照片的高度。只读。</span><span class="sxs-lookup"><span data-stu-id="9022d-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="9022d-132">width</span><span class="sxs-lookup"><span data-stu-id="9022d-132">width</span></span>|<span data-ttu-id="9022d-133">int32</span><span class="sxs-lookup"><span data-stu-id="9022d-133">int32</span></span>|<span data-ttu-id="9022d-p105">照片的宽度。只读。</span><span class="sxs-lookup"><span data-stu-id="9022d-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9022d-136">关系</span><span class="sxs-lookup"><span data-stu-id="9022d-136">Relationships</span></span>
<span data-ttu-id="9022d-137">无</span><span class="sxs-lookup"><span data-stu-id="9022d-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9022d-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9022d-138">JSON representation</span></span>

<span data-ttu-id="9022d-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9022d-139">Here is a JSON representation of the resource.</span></span>

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

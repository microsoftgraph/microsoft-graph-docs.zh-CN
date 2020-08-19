---
title: profilePhoto 资源类型
description: 从 Exchange Online 或 Azure Active Directory (AAD) 中访问的用户、组或 Outlook 联系人的个人资料照片。二进制数据未在 base-64 中进行编码。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: dbaff3f61e7c430ae77ec10bea66a9c11dabaf05
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812034"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="a8530-104">profilePhoto 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8530-104">profilePhoto resource type</span></span>

<span data-ttu-id="a8530-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8530-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8530-p102">从 Exchange Online 或 Azure Active Directory (AAD) 中访问的用户、组或 Outlook 联系人的个人资料照片。二进制数据未在 base-64 中进行编码。</span><span class="sxs-lookup"><span data-stu-id="a8530-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD). It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="a8530-108">Exchange Online 支持的 HD 照片大小如下所示：'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504' 和 '648x648'。</span><span class="sxs-lookup"><span data-stu-id="a8530-108">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="a8530-109">在 AAD 上，照片可以是任何维度。</span><span class="sxs-lookup"><span data-stu-id="a8530-109">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="a8530-110">方法</span><span class="sxs-lookup"><span data-stu-id="a8530-110">Methods</span></span>

| <span data-ttu-id="a8530-111">方法</span><span class="sxs-lookup"><span data-stu-id="a8530-111">Method</span></span>       | <span data-ttu-id="a8530-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="a8530-112">Return Type</span></span>  |<span data-ttu-id="a8530-113">说明</span><span class="sxs-lookup"><span data-stu-id="a8530-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a8530-114">获取 profilePhoto</span><span class="sxs-lookup"><span data-stu-id="a8530-114">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="a8530-115">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="a8530-115">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="a8530-116">获取指定的 **profilePhoto** 或其元数据（**profilePhoto** 属性）。</span><span class="sxs-lookup"><span data-stu-id="a8530-116">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="a8530-117">更新</span><span class="sxs-lookup"><span data-stu-id="a8530-117">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="a8530-118">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="a8530-118">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="a8530-p104">将照片分配给指定的用户、组或联系人。照片应为二进制格式。它将替换现有的照片（如有）。</span><span class="sxs-lookup"><span data-stu-id="a8530-p104">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="a8530-122">属性</span><span class="sxs-lookup"><span data-stu-id="a8530-122">Properties</span></span>
| <span data-ttu-id="a8530-123">属性</span><span class="sxs-lookup"><span data-stu-id="a8530-123">Property</span></span>     | <span data-ttu-id="a8530-124">类型</span><span class="sxs-lookup"><span data-stu-id="a8530-124">Type</span></span>   |<span data-ttu-id="a8530-125">说明</span><span class="sxs-lookup"><span data-stu-id="a8530-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8530-126">id</span><span class="sxs-lookup"><span data-stu-id="a8530-126">id</span></span>|<span data-ttu-id="a8530-127">string</span><span class="sxs-lookup"><span data-stu-id="a8530-127">string</span></span>|<span data-ttu-id="a8530-128">只读。</span><span class="sxs-lookup"><span data-stu-id="a8530-128">Read-only.</span></span>|
|<span data-ttu-id="a8530-129">height</span><span class="sxs-lookup"><span data-stu-id="a8530-129">height</span></span>|<span data-ttu-id="a8530-130">int32</span><span class="sxs-lookup"><span data-stu-id="a8530-130">int32</span></span>|<span data-ttu-id="a8530-p105">照片的高度。只读。</span><span class="sxs-lookup"><span data-stu-id="a8530-p105">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="a8530-133">width</span><span class="sxs-lookup"><span data-stu-id="a8530-133">width</span></span>|<span data-ttu-id="a8530-134">int32</span><span class="sxs-lookup"><span data-stu-id="a8530-134">int32</span></span>|<span data-ttu-id="a8530-p106">照片的宽度。只读。</span><span class="sxs-lookup"><span data-stu-id="a8530-p106">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8530-137">关系</span><span class="sxs-lookup"><span data-stu-id="a8530-137">Relationships</span></span>
<span data-ttu-id="a8530-138">无</span><span class="sxs-lookup"><span data-stu-id="a8530-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a8530-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8530-139">JSON representation</span></span>

<span data-ttu-id="a8530-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8530-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

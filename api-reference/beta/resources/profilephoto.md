---
title: profilePhoto 资源类型
description: 用户、组或从 Exchange Online 或 Azure Active Directory (AAD) 访问的 Outlook 联系人的个人资料照片。 它是不以 base-64 编码的二进制数据。
localization_priority: Normal
ms.openlocfilehash: edff2919192403b41096a6f9dfcd6dbdcf1446ed
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344074"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="a613f-104">profilePhoto 资源类型</span><span class="sxs-lookup"><span data-stu-id="a613f-104">profilePhoto resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a613f-105">用户、组或从 Exchange Online 或 Azure Active Directory (AAD) 访问的 Outlook 联系人的个人资料照片。</span><span class="sxs-lookup"><span data-stu-id="a613f-105">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="a613f-106">它是不以 base-64 编码的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="a613f-106">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="a613f-107">Exchange Online 支持的 HD 照片大小如下所示：'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504' 和 '648x648'。</span><span class="sxs-lookup"><span data-stu-id="a613f-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="a613f-108">在 AAD 上, 照片可以是任何维度。</span><span class="sxs-lookup"><span data-stu-id="a613f-108">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="a613f-109">方法</span><span class="sxs-lookup"><span data-stu-id="a613f-109">Methods</span></span>

| <span data-ttu-id="a613f-110">方法</span><span class="sxs-lookup"><span data-stu-id="a613f-110">Method</span></span>       | <span data-ttu-id="a613f-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="a613f-111">Return Type</span></span>  |<span data-ttu-id="a613f-112">说明</span><span class="sxs-lookup"><span data-stu-id="a613f-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a613f-113">获取 profilePhoto</span><span class="sxs-lookup"><span data-stu-id="a613f-113">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="a613f-114">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="a613f-114">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="a613f-115">获取指定的 **profilePhoto** 或其元数据（**profilePhoto** 属性）。</span><span class="sxs-lookup"><span data-stu-id="a613f-115">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="a613f-116">更新</span><span class="sxs-lookup"><span data-stu-id="a613f-116">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="a613f-117">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="a613f-117">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="a613f-p104">将照片分配给指定的用户、组或联系人。照片应为二进制格式。它将替换现有的照片（如有）。</span><span class="sxs-lookup"><span data-stu-id="a613f-p104">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="a613f-121">属性</span><span class="sxs-lookup"><span data-stu-id="a613f-121">Properties</span></span>
| <span data-ttu-id="a613f-122">属性</span><span class="sxs-lookup"><span data-stu-id="a613f-122">Property</span></span>     | <span data-ttu-id="a613f-123">类型</span><span class="sxs-lookup"><span data-stu-id="a613f-123">Type</span></span>   |<span data-ttu-id="a613f-124">说明</span><span class="sxs-lookup"><span data-stu-id="a613f-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a613f-125">id</span><span class="sxs-lookup"><span data-stu-id="a613f-125">id</span></span>|<span data-ttu-id="a613f-126">string</span><span class="sxs-lookup"><span data-stu-id="a613f-126">string</span></span>|<span data-ttu-id="a613f-127">只读。</span><span class="sxs-lookup"><span data-stu-id="a613f-127">Read-only.</span></span>|
|<span data-ttu-id="a613f-128">height</span><span class="sxs-lookup"><span data-stu-id="a613f-128">height</span></span>|<span data-ttu-id="a613f-129">时会</span><span class="sxs-lookup"><span data-stu-id="a613f-129">int32</span></span>|<span data-ttu-id="a613f-p105">照片的高度。只读。</span><span class="sxs-lookup"><span data-stu-id="a613f-p105">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="a613f-132">width</span><span class="sxs-lookup"><span data-stu-id="a613f-132">width</span></span>|<span data-ttu-id="a613f-133">时会</span><span class="sxs-lookup"><span data-stu-id="a613f-133">int32</span></span>|<span data-ttu-id="a613f-p106">照片的宽度。只读。</span><span class="sxs-lookup"><span data-stu-id="a613f-p106">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a613f-136">关系</span><span class="sxs-lookup"><span data-stu-id="a613f-136">Relationships</span></span>
<span data-ttu-id="a613f-137">无</span><span class="sxs-lookup"><span data-stu-id="a613f-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a613f-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a613f-138">JSON representation</span></span>

<span data-ttu-id="a613f-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a613f-139">Here is a JSON representation of the resource.</span></span>

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

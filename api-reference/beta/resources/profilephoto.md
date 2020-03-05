---
title: profilePhoto 资源类型
description: 用户、组或从 Exchange Online 或 Azure Active Directory （AAD）访问的 Outlook 联系人的个人资料照片。二进制数据未在 base-64 中进行编码。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9f7d582c64e600846a17654623ca233d0132e6bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521458"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="faf47-104">profilePhoto 资源类型</span><span class="sxs-lookup"><span data-stu-id="faf47-104">profilePhoto resource type</span></span>

<span data-ttu-id="faf47-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="faf47-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="faf47-106">用户、组或从 Exchange Online 或 Azure Active Directory （AAD）访问的 Outlook 联系人的个人资料照片。</span><span class="sxs-lookup"><span data-stu-id="faf47-106">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="faf47-107">它是不以 base-64 编码的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="faf47-107">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="faf47-108">Exchange Online 支持的 HD 照片大小如下所示：'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504' 和 '648x648'。</span><span class="sxs-lookup"><span data-stu-id="faf47-108">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="faf47-109">在 AAD 上，照片可以是任何维度。</span><span class="sxs-lookup"><span data-stu-id="faf47-109">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="faf47-110">方法</span><span class="sxs-lookup"><span data-stu-id="faf47-110">Methods</span></span>

| <span data-ttu-id="faf47-111">方法</span><span class="sxs-lookup"><span data-stu-id="faf47-111">Method</span></span>       | <span data-ttu-id="faf47-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="faf47-112">Return Type</span></span>  |<span data-ttu-id="faf47-113">说明</span><span class="sxs-lookup"><span data-stu-id="faf47-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="faf47-114">获取 profilePhoto</span><span class="sxs-lookup"><span data-stu-id="faf47-114">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="faf47-115">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="faf47-115">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="faf47-116">获取指定的 **profilePhoto** 或其元数据（**profilePhoto** 属性）。</span><span class="sxs-lookup"><span data-stu-id="faf47-116">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="faf47-117">更新</span><span class="sxs-lookup"><span data-stu-id="faf47-117">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="faf47-118">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="faf47-118">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="faf47-p104">将照片分配给指定的用户、组或联系人。照片应为二进制格式。它将替换现有的照片（如有）。</span><span class="sxs-lookup"><span data-stu-id="faf47-p104">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="faf47-122">属性</span><span class="sxs-lookup"><span data-stu-id="faf47-122">Properties</span></span>
| <span data-ttu-id="faf47-123">属性</span><span class="sxs-lookup"><span data-stu-id="faf47-123">Property</span></span>     | <span data-ttu-id="faf47-124">类型</span><span class="sxs-lookup"><span data-stu-id="faf47-124">Type</span></span>   |<span data-ttu-id="faf47-125">说明</span><span class="sxs-lookup"><span data-stu-id="faf47-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="faf47-126">id</span><span class="sxs-lookup"><span data-stu-id="faf47-126">id</span></span>|<span data-ttu-id="faf47-127">string</span><span class="sxs-lookup"><span data-stu-id="faf47-127">string</span></span>|<span data-ttu-id="faf47-128">只读。</span><span class="sxs-lookup"><span data-stu-id="faf47-128">Read-only.</span></span>|
|<span data-ttu-id="faf47-129">height</span><span class="sxs-lookup"><span data-stu-id="faf47-129">height</span></span>|<span data-ttu-id="faf47-130">int32</span><span class="sxs-lookup"><span data-stu-id="faf47-130">int32</span></span>|<span data-ttu-id="faf47-p105">照片的高度。只读。</span><span class="sxs-lookup"><span data-stu-id="faf47-p105">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="faf47-133">width</span><span class="sxs-lookup"><span data-stu-id="faf47-133">width</span></span>|<span data-ttu-id="faf47-134">int32</span><span class="sxs-lookup"><span data-stu-id="faf47-134">int32</span></span>|<span data-ttu-id="faf47-p106">照片的宽度。只读。</span><span class="sxs-lookup"><span data-stu-id="faf47-p106">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="faf47-137">关系</span><span class="sxs-lookup"><span data-stu-id="faf47-137">Relationships</span></span>
<span data-ttu-id="faf47-138">无</span><span class="sxs-lookup"><span data-stu-id="faf47-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="faf47-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="faf47-139">JSON representation</span></span>

<span data-ttu-id="faf47-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="faf47-140">Here is a JSON representation of the resource.</span></span>

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

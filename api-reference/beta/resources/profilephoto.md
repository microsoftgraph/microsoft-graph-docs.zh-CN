---
title: profilePhoto 资源类型
description: 用户、 组或 Outlook 联系人从 Exchange Online 或 Azure Active Directory (AAD) 访问的配置文件照片。 它是未使用 base64 编码的二进制数据。
ms.openlocfilehash: 61123542ce66c1e999fb6d90c154a78dbb77df50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042571"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="e59f6-104">profilePhoto 资源类型</span><span class="sxs-lookup"><span data-stu-id="e59f6-104">profilePhoto resource type</span></span>

> <span data-ttu-id="e59f6-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e59f6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e59f6-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e59f6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e59f6-107">用户、 组或 Outlook 联系人从 Exchange Online 或 Azure Active Directory (AAD) 访问的配置文件照片。</span><span class="sxs-lookup"><span data-stu-id="e59f6-107">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="e59f6-108">它是未使用 base64 编码的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="e59f6-108">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="e59f6-109">Exchange Online 支持的 HD 照片大小如下所示：'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504' 和 '648x648'。</span><span class="sxs-lookup"><span data-stu-id="e59f6-109">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="e59f6-110">在 AAD，照片可以是任何维度。</span><span class="sxs-lookup"><span data-stu-id="e59f6-110">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="e59f6-111">方法</span><span class="sxs-lookup"><span data-stu-id="e59f6-111">Methods</span></span>

| <span data-ttu-id="e59f6-112">方法</span><span class="sxs-lookup"><span data-stu-id="e59f6-112">Method</span></span>       | <span data-ttu-id="e59f6-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="e59f6-113">Return Type</span></span>  |<span data-ttu-id="e59f6-114">说明</span><span class="sxs-lookup"><span data-stu-id="e59f6-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e59f6-115">获取 profilePhoto</span><span class="sxs-lookup"><span data-stu-id="e59f6-115">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="e59f6-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="e59f6-116">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="e59f6-117">获取指定的**profilePhoto**或其元数据 （**profilePhoto**属性）。</span><span class="sxs-lookup"><span data-stu-id="e59f6-117">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="e59f6-118">更新</span><span class="sxs-lookup"><span data-stu-id="e59f6-118">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="e59f6-119">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="e59f6-119">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="e59f6-p105">将照片分配给指定的用户、组或联系人。照片应为二进制格式。它将替换现有的照片（如有）。</span><span class="sxs-lookup"><span data-stu-id="e59f6-p105">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="e59f6-123">属性</span><span class="sxs-lookup"><span data-stu-id="e59f6-123">Properties</span></span>
| <span data-ttu-id="e59f6-124">属性</span><span class="sxs-lookup"><span data-stu-id="e59f6-124">Property</span></span>     | <span data-ttu-id="e59f6-125">类型</span><span class="sxs-lookup"><span data-stu-id="e59f6-125">Type</span></span>   |<span data-ttu-id="e59f6-126">说明</span><span class="sxs-lookup"><span data-stu-id="e59f6-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e59f6-127">ID</span><span class="sxs-lookup"><span data-stu-id="e59f6-127">id</span></span>|<span data-ttu-id="e59f6-128">string</span><span class="sxs-lookup"><span data-stu-id="e59f6-128">string</span></span>|<span data-ttu-id="e59f6-129">只读。</span><span class="sxs-lookup"><span data-stu-id="e59f6-129">Read-only.</span></span>|
|<span data-ttu-id="e59f6-130">height</span><span class="sxs-lookup"><span data-stu-id="e59f6-130">height</span></span>|<span data-ttu-id="e59f6-131">int32</span><span class="sxs-lookup"><span data-stu-id="e59f6-131">int32</span></span>|<span data-ttu-id="e59f6-p106">照片的高度。只读。</span><span class="sxs-lookup"><span data-stu-id="e59f6-p106">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="e59f6-134">width</span><span class="sxs-lookup"><span data-stu-id="e59f6-134">width</span></span>|<span data-ttu-id="e59f6-135">int32</span><span class="sxs-lookup"><span data-stu-id="e59f6-135">int32</span></span>|<span data-ttu-id="e59f6-p107">照片的宽度。只读。</span><span class="sxs-lookup"><span data-stu-id="e59f6-p107">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e59f6-138">Relationships</span><span class="sxs-lookup"><span data-stu-id="e59f6-138">Relationships</span></span>
<span data-ttu-id="e59f6-139">无</span><span class="sxs-lookup"><span data-stu-id="e59f6-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e59f6-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e59f6-140">JSON representation</span></span>

<span data-ttu-id="e59f6-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e59f6-141">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

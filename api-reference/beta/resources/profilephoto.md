---
title: profilePhoto 资源类型
description: 用户、组或从 Exchange Online 或 Azure Active Directory (AAD) 访问的 Outlook 联系人的个人资料照片。 它是不以 base-64 编码的二进制数据。
localization_priority: Normal
ms.openlocfilehash: 2a831abd098fb9a0dfa95f6d6dd3a9cd5de128cd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563271"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="ecb31-104">profilePhoto 资源类型</span><span class="sxs-lookup"><span data-stu-id="ecb31-104">profilePhoto resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecb31-105">用户、组或从 Exchange Online 或 Azure Active Directory (AAD) 访问的 Outlook 联系人的个人资料照片。</span><span class="sxs-lookup"><span data-stu-id="ecb31-105">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="ecb31-106">它是不以 base-64 编码的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="ecb31-106">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="ecb31-107">Exchange Online 支持的 HD 照片大小如下所示：'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504' 和 '648x648'。</span><span class="sxs-lookup"><span data-stu-id="ecb31-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="ecb31-108">在 AAD 上, 照片可以是任何维度。</span><span class="sxs-lookup"><span data-stu-id="ecb31-108">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="ecb31-109">方法</span><span class="sxs-lookup"><span data-stu-id="ecb31-109">Methods</span></span>

| <span data-ttu-id="ecb31-110">方法</span><span class="sxs-lookup"><span data-stu-id="ecb31-110">Method</span></span>       | <span data-ttu-id="ecb31-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="ecb31-111">Return Type</span></span>  |<span data-ttu-id="ecb31-112">说明</span><span class="sxs-lookup"><span data-stu-id="ecb31-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ecb31-113">获取 profilePhoto</span><span class="sxs-lookup"><span data-stu-id="ecb31-113">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="ecb31-114">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="ecb31-114">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="ecb31-115">获取指定的 **profilePhoto** 或其元数据（**profilePhoto** 属性）。</span><span class="sxs-lookup"><span data-stu-id="ecb31-115">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="ecb31-116">更新</span><span class="sxs-lookup"><span data-stu-id="ecb31-116">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="ecb31-117">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="ecb31-117">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="ecb31-p104">将照片分配给指定的用户、组或联系人。照片应为二进制格式。它将替换现有的照片（如有）。</span><span class="sxs-lookup"><span data-stu-id="ecb31-p104">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="ecb31-121">属性</span><span class="sxs-lookup"><span data-stu-id="ecb31-121">Properties</span></span>
| <span data-ttu-id="ecb31-122">属性</span><span class="sxs-lookup"><span data-stu-id="ecb31-122">Property</span></span>     | <span data-ttu-id="ecb31-123">类型</span><span class="sxs-lookup"><span data-stu-id="ecb31-123">Type</span></span>   |<span data-ttu-id="ecb31-124">说明</span><span class="sxs-lookup"><span data-stu-id="ecb31-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecb31-125">id</span><span class="sxs-lookup"><span data-stu-id="ecb31-125">id</span></span>|<span data-ttu-id="ecb31-126">string</span><span class="sxs-lookup"><span data-stu-id="ecb31-126">string</span></span>|<span data-ttu-id="ecb31-127">只读。</span><span class="sxs-lookup"><span data-stu-id="ecb31-127">Read-only.</span></span>|
|<span data-ttu-id="ecb31-128">height</span><span class="sxs-lookup"><span data-stu-id="ecb31-128">height</span></span>|<span data-ttu-id="ecb31-129">时会</span><span class="sxs-lookup"><span data-stu-id="ecb31-129">int32</span></span>|<span data-ttu-id="ecb31-p105">照片的高度。只读。</span><span class="sxs-lookup"><span data-stu-id="ecb31-p105">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="ecb31-132">width</span><span class="sxs-lookup"><span data-stu-id="ecb31-132">width</span></span>|<span data-ttu-id="ecb31-133">时会</span><span class="sxs-lookup"><span data-stu-id="ecb31-133">int32</span></span>|<span data-ttu-id="ecb31-p106">照片的宽度。只读。</span><span class="sxs-lookup"><span data-stu-id="ecb31-p106">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecb31-136">关系</span><span class="sxs-lookup"><span data-stu-id="ecb31-136">Relationships</span></span>
<span data-ttu-id="ecb31-137">无</span><span class="sxs-lookup"><span data-stu-id="ecb31-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ecb31-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ecb31-138">JSON representation</span></span>

<span data-ttu-id="ecb31-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ecb31-139">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/profilephoto.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

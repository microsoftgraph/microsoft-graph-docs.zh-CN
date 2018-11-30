---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
ms.openlocfilehash: 922f87c77280627efb956e4558e1ff269daa9311
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045789"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="65dc5-102">ContentTypeInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="65dc5-102">ContentTypeInfo resource type</span></span>

> <span data-ttu-id="65dc5-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="65dc5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65dc5-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="65dc5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65dc5-105">**contentTypeInfo** 资源指示项的 SharePoint 内容类型。</span><span class="sxs-lookup"><span data-stu-id="65dc5-105">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="65dc5-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65dc5-106">JSON representation</span></span>

<span data-ttu-id="65dc5-107">下面是 **contentTypeInfo** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65dc5-107">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="65dc5-108">属性</span><span class="sxs-lookup"><span data-stu-id="65dc5-108">Properties</span></span>

| <span data-ttu-id="65dc5-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="65dc5-109">Property name</span></span>  | <span data-ttu-id="65dc5-110">类型</span><span class="sxs-lookup"><span data-stu-id="65dc5-110">Type</span></span>    | <span data-ttu-id="65dc5-111">说明</span><span class="sxs-lookup"><span data-stu-id="65dc5-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="65dc5-112">**id**</span><span class="sxs-lookup"><span data-stu-id="65dc5-112">**id**</span></span>         | <span data-ttu-id="65dc5-113">string</span><span class="sxs-lookup"><span data-stu-id="65dc5-113">string</span></span>  | <span data-ttu-id="65dc5-114">内容类型的 ID。</span><span class="sxs-lookup"><span data-stu-id="65dc5-114">The id of the content type.</span></span>
| <span data-ttu-id="65dc5-115">**name**</span><span class="sxs-lookup"><span data-stu-id="65dc5-115">**name**</span></span>       | <span data-ttu-id="65dc5-116">string</span><span class="sxs-lookup"><span data-stu-id="65dc5-116">string</span></span>  | <span data-ttu-id="65dc5-117">内容类型的名称。</span><span class="sxs-lookup"><span data-stu-id="65dc5-117">The name of the content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo"
} -->

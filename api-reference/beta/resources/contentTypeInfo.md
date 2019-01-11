---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
ms.openlocfilehash: e394d52a5f7ed5e8dce1c61d31d787d62bd36e56
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892335"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="61c5c-102">ContentTypeInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="61c5c-102">ContentTypeInfo resource type</span></span>

> <span data-ttu-id="61c5c-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="61c5c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61c5c-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="61c5c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61c5c-105">**contentTypeInfo** 资源指示项的 SharePoint 内容类型。</span><span class="sxs-lookup"><span data-stu-id="61c5c-105">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="61c5c-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61c5c-106">JSON representation</span></span>

<span data-ttu-id="61c5c-107">下面是 **contentTypeInfo** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61c5c-107">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="61c5c-108">属性</span><span class="sxs-lookup"><span data-stu-id="61c5c-108">Properties</span></span>

| <span data-ttu-id="61c5c-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="61c5c-109">Property name</span></span>  | <span data-ttu-id="61c5c-110">类型</span><span class="sxs-lookup"><span data-stu-id="61c5c-110">Type</span></span>    | <span data-ttu-id="61c5c-111">说明</span><span class="sxs-lookup"><span data-stu-id="61c5c-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="61c5c-112">**id**</span><span class="sxs-lookup"><span data-stu-id="61c5c-112">**id**</span></span>         | <span data-ttu-id="61c5c-113">string</span><span class="sxs-lookup"><span data-stu-id="61c5c-113">string</span></span>  | <span data-ttu-id="61c5c-114">内容类型的 ID。</span><span class="sxs-lookup"><span data-stu-id="61c5c-114">The id of the content type.</span></span>
| <span data-ttu-id="61c5c-115">**name**</span><span class="sxs-lookup"><span data-stu-id="61c5c-115">**name**</span></span>       | <span data-ttu-id="61c5c-116">string</span><span class="sxs-lookup"><span data-stu-id="61c5c-116">string</span></span>  | <span data-ttu-id="61c5c-117">内容类型的名称。</span><span class="sxs-lookup"><span data-stu-id="61c5c-117">The name of the content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo"
} -->

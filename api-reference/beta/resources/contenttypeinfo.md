---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
ms.openlocfilehash: 107dfb3577489521d2e10e0c8fd2fe52c4f90b10
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341221"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="fa433-102">ContentTypeInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa433-102">ContentTypeInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa433-103">**contentTypeInfo** 资源指示项的 SharePoint 内容类型。</span><span class="sxs-lookup"><span data-stu-id="fa433-103">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa433-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa433-104">JSON representation</span></span>

<span data-ttu-id="fa433-105">下面是 **contentTypeInfo** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa433-105">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="fa433-106">属性</span><span class="sxs-lookup"><span data-stu-id="fa433-106">Properties</span></span>

| <span data-ttu-id="fa433-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="fa433-107">Property name</span></span>  | <span data-ttu-id="fa433-108">类型</span><span class="sxs-lookup"><span data-stu-id="fa433-108">Type</span></span>    | <span data-ttu-id="fa433-109">说明</span><span class="sxs-lookup"><span data-stu-id="fa433-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="fa433-110">**id**</span><span class="sxs-lookup"><span data-stu-id="fa433-110">**id**</span></span>         | <span data-ttu-id="fa433-111">string</span><span class="sxs-lookup"><span data-stu-id="fa433-111">string</span></span>  | <span data-ttu-id="fa433-112">内容类型的 ID。</span><span class="sxs-lookup"><span data-stu-id="fa433-112">The id of the content type.</span></span>
| <span data-ttu-id="fa433-113">**name**</span><span class="sxs-lookup"><span data-stu-id="fa433-113">**name**</span></span>       | <span data-ttu-id="fa433-114">string</span><span class="sxs-lookup"><span data-stu-id="fa433-114">string</span></span>  | <span data-ttu-id="fa433-115">内容类型的名称。</span><span class="sxs-lookup"><span data-stu-id="fa433-115">The name of the content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo",
  "suppressions": []
}
-->

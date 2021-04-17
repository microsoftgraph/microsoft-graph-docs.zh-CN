---
title: teamsAppIcon 资源类型
description: 与 Microsoft Teams 上的应用相关联的图标。
author: jecha
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3e8a256dc0b9e92c414cd3d362bb36579708083f
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882652"
---
# <a name="teamsappicon-resource-type"></a><span data-ttu-id="3d730-103">teamsAppIcon 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d730-103">teamsAppIcon resource type</span></span>

<span data-ttu-id="3d730-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d730-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d730-105">与 [teamsApp](teamsapp.md)相关联的图标。</span><span class="sxs-lookup"><span data-stu-id="3d730-105">An icon associated with a [teamsApp](teamsapp.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3d730-106">方法</span><span class="sxs-lookup"><span data-stu-id="3d730-106">Methods</span></span>

| <span data-ttu-id="3d730-107">方法</span><span class="sxs-lookup"><span data-stu-id="3d730-107">Method</span></span>                                            | <span data-ttu-id="3d730-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3d730-108">Return Type</span></span>                                       | <span data-ttu-id="3d730-109">说明</span><span class="sxs-lookup"><span data-stu-id="3d730-109">Description</span></span>                                                    | 
| :------------------------------------------------ | :------------------------------------------------ | :------------------------------------------------------------- |
| [<span data-ttu-id="3d730-110">获取图标</span><span class="sxs-lookup"><span data-stu-id="3d730-110">Get icon</span></span>](../api/teamsappicon-get.md)     | [<span data-ttu-id="3d730-111">teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="3d730-111">teamsAppIcon</span></span>](teamsappicon.md)                   | <span data-ttu-id="3d730-112">获取与 Teams 应用的特定版本相关联的图标。</span><span class="sxs-lookup"><span data-stu-id="3d730-112">Get an icon associated with a specific version of a Teams app.</span></span> |
| [<span data-ttu-id="3d730-113">获取托管内容</span><span class="sxs-lookup"><span data-stu-id="3d730-113">Get hosted content</span></span>](../api/teamworkhostedcontent-get.md) | [<span data-ttu-id="3d730-114">teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="3d730-114">teamworkHostedContent</span></span>](teamworkhostedcontent.md) | <span data-ttu-id="3d730-115">获取托管内容 (及其字节数) 图标的字节数。</span><span class="sxs-lookup"><span data-stu-id="3d730-115">Get hosted content (and its bytes) for an icon.</span></span>                |

## <a name="properties"></a><span data-ttu-id="3d730-116">属性</span><span class="sxs-lookup"><span data-stu-id="3d730-116">Properties</span></span>

| <span data-ttu-id="3d730-117">属性</span><span class="sxs-lookup"><span data-stu-id="3d730-117">Property</span></span>      | <span data-ttu-id="3d730-118">类型</span><span class="sxs-lookup"><span data-stu-id="3d730-118">Type</span></span>                        | <span data-ttu-id="3d730-119">说明</span><span class="sxs-lookup"><span data-stu-id="3d730-119">Description</span></span>                                                                             |
| :------------ | :-------------------------- | :-------------------------------------------------------------------------------------- |
| <span data-ttu-id="3d730-120">id</span><span class="sxs-lookup"><span data-stu-id="3d730-120">id</span></span>            | <span data-ttu-id="3d730-121">string</span><span class="sxs-lookup"><span data-stu-id="3d730-121">string</span></span>                      | <span data-ttu-id="3d730-122">应用图标的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="3d730-122">The unique ID of the app icon.</span></span>                                                          |
| <span data-ttu-id="3d730-123">webUrl</span><span class="sxs-lookup"><span data-stu-id="3d730-123">webUrl</span></span>        | <span data-ttu-id="3d730-124">string</span><span class="sxs-lookup"><span data-stu-id="3d730-124">string</span></span>                      | <span data-ttu-id="3d730-125">可用于下载图像的 Web URL。</span><span class="sxs-lookup"><span data-stu-id="3d730-125">The web URL that can be used for downloading the image.</span></span>                                 |

## <a name="relationships"></a><span data-ttu-id="3d730-126">关系</span><span class="sxs-lookup"><span data-stu-id="3d730-126">Relationships</span></span>

| <span data-ttu-id="3d730-127">关系</span><span class="sxs-lookup"><span data-stu-id="3d730-127">Relationship</span></span>  | <span data-ttu-id="3d730-128">类型</span><span class="sxs-lookup"><span data-stu-id="3d730-128">Type</span></span>                                              | <span data-ttu-id="3d730-129">说明</span><span class="sxs-lookup"><span data-stu-id="3d730-129">Description</span></span>                                                                         |
| :------------ | :------------------------------------------------ | :---------------------------------------------------------------------------------- |
| <span data-ttu-id="3d730-130">hostedContent</span><span class="sxs-lookup"><span data-stu-id="3d730-130">hostedContent</span></span> | [<span data-ttu-id="3d730-131">teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="3d730-131">teamworkHostedContent</span></span>](teamworkhostedcontent.md) | <span data-ttu-id="3d730-132">如果图标托管在 Teams 基础结构中，则应用图标的内容。</span><span class="sxs-lookup"><span data-stu-id="3d730-132">The contents of the app icon if the icon is hosted within the Teams infrastructure.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3d730-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d730-133">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppIcon",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "webUrl": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="3d730-134">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3d730-134">See also</span></span>

- [<span data-ttu-id="3d730-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="3d730-135">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="3d730-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="3d730-136">teamsAppDefinition</span></span>](teamsappdefinition.md)

---
title: teamsTabConfiguration 资源类型 (开放式类型)
description: 确定选项卡内容的设置。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: beeb9c6b06457795b802e18a1a2f7fac909e0c6c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345712"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="522b7-103">teamsTabConfiguration 资源类型 (开放式类型)</span><span class="sxs-lookup"><span data-stu-id="522b7-103">teamsTabConfiguration resource type (Open Type)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="522b7-104">确定[选项卡](teamstab.md)内容的设置。以交互方式配置选项卡时, 选项卡提供程序应用程序将设置此信息。</span><span class="sxs-lookup"><span data-stu-id="522b7-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="522b7-105">除了以下属性之外, 一些选项卡提供程序应用程序还指定其他自定义属性。</span><span class="sxs-lookup"><span data-stu-id="522b7-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="522b7-106">属性</span><span class="sxs-lookup"><span data-stu-id="522b7-106">Properties</span></span>

|<span data-ttu-id="522b7-107">属性</span><span class="sxs-lookup"><span data-stu-id="522b7-107">Property</span></span>|<span data-ttu-id="522b7-108">类型</span><span class="sxs-lookup"><span data-stu-id="522b7-108">Type</span></span>|<span data-ttu-id="522b7-109">说明</span><span class="sxs-lookup"><span data-stu-id="522b7-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="522b7-110">entityId</span><span class="sxs-lookup"><span data-stu-id="522b7-110">entityId</span></span>   |   <span data-ttu-id="522b7-111">string</span><span class="sxs-lookup"><span data-stu-id="522b7-111">string</span></span> |  <span data-ttu-id="522b7-112">由选项卡提供程序承载的实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="522b7-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="522b7-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="522b7-113">contentUrl</span></span> |   <span data-ttu-id="522b7-114">string</span><span class="sxs-lookup"><span data-stu-id="522b7-114">string</span></span> |  <span data-ttu-id="522b7-115">用于在团队中呈现选项卡内容的 Url。</span><span class="sxs-lookup"><span data-stu-id="522b7-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="522b7-116">必填。</span><span class="sxs-lookup"><span data-stu-id="522b7-116">Required.</span></span>    |
|  <span data-ttu-id="522b7-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="522b7-117">removeUrl</span></span>  |   <span data-ttu-id="522b7-118">string</span><span class="sxs-lookup"><span data-stu-id="522b7-118">string</span></span> |  <span data-ttu-id="522b7-119">使用团队客户端删除选项卡时, 由团队客户端调用的 Url。</span><span class="sxs-lookup"><span data-stu-id="522b7-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="522b7-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="522b7-120">websiteUrl</span></span> |   <span data-ttu-id="522b7-121">string</span><span class="sxs-lookup"><span data-stu-id="522b7-121">string</span></span> |  <span data-ttu-id="522b7-122">用于显示团队外部的选项卡内容的 Url。</span><span class="sxs-lookup"><span data-stu-id="522b7-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="522b7-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="522b7-123">JSON representation</span></span>

<span data-ttu-id="522b7-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="522b7-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

---
title: 'teamsTabConfiguration 资源类型 (开放类型) '
description: 确定选项卡内容的设置。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e81813f408c561a09b89e4cb3fd490acb6988cff
ms.sourcegitcommit: c7c198f6fa252b68e91be341b93b818afd387486
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2020
ms.locfileid: "47439988"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="0dac4-103">teamsTabConfiguration 资源类型 (开放类型) </span><span class="sxs-lookup"><span data-stu-id="0dac4-103">teamsTabConfiguration resource type (Open Type)</span></span>

<span data-ttu-id="0dac4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dac4-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="0dac4-105">确定 [选项卡](teamstab.md)内容的设置。以交互方式配置选项卡时，选项卡提供程序应用程序将设置此信息。</span><span class="sxs-lookup"><span data-stu-id="0dac4-105">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="0dac4-106">除了以下属性之外，一些选项卡提供程序应用程序还指定其他自定义属性。</span><span class="sxs-lookup"><span data-stu-id="0dac4-106">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="0dac4-107">属性</span><span class="sxs-lookup"><span data-stu-id="0dac4-107">Properties</span></span>

|<span data-ttu-id="0dac4-108">属性</span><span class="sxs-lookup"><span data-stu-id="0dac4-108">Property</span></span>|<span data-ttu-id="0dac4-109">类型</span><span class="sxs-lookup"><span data-stu-id="0dac4-109">Type</span></span>|<span data-ttu-id="0dac4-110">Description</span><span class="sxs-lookup"><span data-stu-id="0dac4-110">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="0dac4-111">entityId</span><span class="sxs-lookup"><span data-stu-id="0dac4-111">entityId</span></span>   |   <span data-ttu-id="0dac4-112">string</span><span class="sxs-lookup"><span data-stu-id="0dac4-112">string</span></span> |  <span data-ttu-id="0dac4-113">由选项卡提供程序承载的实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="0dac4-113">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="0dac4-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="0dac4-114">contentUrl</span></span> |   <span data-ttu-id="0dac4-115">string</span><span class="sxs-lookup"><span data-stu-id="0dac4-115">string</span></span> |  <span data-ttu-id="0dac4-116">用于在团队中呈现选项卡内容的 Url。</span><span class="sxs-lookup"><span data-stu-id="0dac4-116">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="0dac4-117">必需。</span><span class="sxs-lookup"><span data-stu-id="0dac4-117">Required.</span></span>    |
|  <span data-ttu-id="0dac4-118">removeUrl</span><span class="sxs-lookup"><span data-stu-id="0dac4-118">removeUrl</span></span>  |   <span data-ttu-id="0dac4-119">string</span><span class="sxs-lookup"><span data-stu-id="0dac4-119">string</span></span> |  <span data-ttu-id="0dac4-120">使用团队客户端删除选项卡时，由团队客户端调用的 Url。</span><span class="sxs-lookup"><span data-stu-id="0dac4-120">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="0dac4-121">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="0dac4-121">websiteUrl</span></span> |   <span data-ttu-id="0dac4-122">string</span><span class="sxs-lookup"><span data-stu-id="0dac4-122">string</span></span> |  <span data-ttu-id="0dac4-123">用于显示团队外部的选项卡内容的 Url。</span><span class="sxs-lookup"><span data-stu-id="0dac4-123">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="0dac4-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0dac4-124">JSON representation</span></span>

<span data-ttu-id="0dac4-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0dac4-125">The following is a JSON representation of the resource.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

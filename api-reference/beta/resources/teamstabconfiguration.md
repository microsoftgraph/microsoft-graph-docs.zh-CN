---
title: teamsTabConfiguration 资源类型 (开放式类型)
description: 确定选项卡内容的设置。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 10cc22e70288d1643a3a2cdebe23a012e22e3879
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550737"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="75d8e-103">teamsTabConfiguration 资源类型 (开放式类型)</span><span class="sxs-lookup"><span data-stu-id="75d8e-103">teamsTabConfiguration resource type (Open Type)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75d8e-104">确定[选项卡](teamstab.md)内容的设置。以交互方式配置选项卡时, 选项卡提供程序应用程序将设置此信息。</span><span class="sxs-lookup"><span data-stu-id="75d8e-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="75d8e-105">除了以下属性之外, 一些选项卡提供程序应用程序还指定其他自定义属性。</span><span class="sxs-lookup"><span data-stu-id="75d8e-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="75d8e-106">属性</span><span class="sxs-lookup"><span data-stu-id="75d8e-106">Properties</span></span>

|<span data-ttu-id="75d8e-107">属性</span><span class="sxs-lookup"><span data-stu-id="75d8e-107">Property</span></span>|<span data-ttu-id="75d8e-108">类型</span><span class="sxs-lookup"><span data-stu-id="75d8e-108">Type</span></span>|<span data-ttu-id="75d8e-109">说明</span><span class="sxs-lookup"><span data-stu-id="75d8e-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="75d8e-110">entityId</span><span class="sxs-lookup"><span data-stu-id="75d8e-110">entityId</span></span>   |   <span data-ttu-id="75d8e-111">string</span><span class="sxs-lookup"><span data-stu-id="75d8e-111">string</span></span> |  <span data-ttu-id="75d8e-112">由选项卡提供程序承载的实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="75d8e-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="75d8e-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="75d8e-113">contentUrl</span></span> |   <span data-ttu-id="75d8e-114">string</span><span class="sxs-lookup"><span data-stu-id="75d8e-114">string</span></span> |  <span data-ttu-id="75d8e-115">用于在团队中呈现选项卡内容的 Url。</span><span class="sxs-lookup"><span data-stu-id="75d8e-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="75d8e-116">必需。</span><span class="sxs-lookup"><span data-stu-id="75d8e-116">Required.</span></span>    |
|  <span data-ttu-id="75d8e-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="75d8e-117">removeUrl</span></span>  |   <span data-ttu-id="75d8e-118">string</span><span class="sxs-lookup"><span data-stu-id="75d8e-118">string</span></span> |  <span data-ttu-id="75d8e-119">使用团队客户端删除选项卡时, 由团队客户端调用的 Url。</span><span class="sxs-lookup"><span data-stu-id="75d8e-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="75d8e-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="75d8e-120">websiteUrl</span></span> |   <span data-ttu-id="75d8e-121">string</span><span class="sxs-lookup"><span data-stu-id="75d8e-121">string</span></span> |  <span data-ttu-id="75d8e-122">用于显示团队外部的选项卡内容的 Url。</span><span class="sxs-lookup"><span data-stu-id="75d8e-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="75d8e-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75d8e-123">JSON representation</span></span>

<span data-ttu-id="75d8e-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75d8e-124">The following is a JSON representation of the resource.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstabconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

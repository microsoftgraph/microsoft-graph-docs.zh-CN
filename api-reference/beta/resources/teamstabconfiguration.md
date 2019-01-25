---
title: teamsTabConfiguration 资源类型 （打开类型）
description: 确定内容的选项卡的设置。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 10cc22e70288d1643a3a2cdebe23a012e22e3879
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519197"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="a96d9-103">teamsTabConfiguration 资源类型 （打开类型）</span><span class="sxs-lookup"><span data-stu-id="a96d9-103">teamsTabConfiguration resource type (Open Type)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a96d9-104">确定内容的[选项卡上](teamstab.md)的设置。选项卡以交互方式配置时，此信息由选项卡提供程序应用程序设置。</span><span class="sxs-lookup"><span data-stu-id="a96d9-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="a96d9-105">除了下面的属性中，某些选项卡提供程序应用程序指定其他自定义属性。</span><span class="sxs-lookup"><span data-stu-id="a96d9-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="a96d9-106">属性</span><span class="sxs-lookup"><span data-stu-id="a96d9-106">Properties</span></span>

|<span data-ttu-id="a96d9-107">属性</span><span class="sxs-lookup"><span data-stu-id="a96d9-107">Property</span></span>|<span data-ttu-id="a96d9-108">类型</span><span class="sxs-lookup"><span data-stu-id="a96d9-108">Type</span></span>|<span data-ttu-id="a96d9-109">说明</span><span class="sxs-lookup"><span data-stu-id="a96d9-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="a96d9-110">entityId</span><span class="sxs-lookup"><span data-stu-id="a96d9-110">entityId</span></span>   |   <span data-ttu-id="a96d9-111">string</span><span class="sxs-lookup"><span data-stu-id="a96d9-111">string</span></span> |  <span data-ttu-id="a96d9-112">选项卡上的服务提供商托管实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="a96d9-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="a96d9-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="a96d9-113">contentUrl</span></span> |   <span data-ttu-id="a96d9-114">string</span><span class="sxs-lookup"><span data-stu-id="a96d9-114">string</span></span> |  <span data-ttu-id="a96d9-115">用于呈现团队中的选项卡内容的 Url。</span><span class="sxs-lookup"><span data-stu-id="a96d9-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="a96d9-116">必需。</span><span class="sxs-lookup"><span data-stu-id="a96d9-116">Required.</span></span>    |
|  <span data-ttu-id="a96d9-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="a96d9-117">removeUrl</span></span>  |   <span data-ttu-id="a96d9-118">string</span><span class="sxs-lookup"><span data-stu-id="a96d9-118">string</span></span> |  <span data-ttu-id="a96d9-119">使用团队客户端中移除一个选项卡时调用团队客户端的 Url。</span><span class="sxs-lookup"><span data-stu-id="a96d9-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="a96d9-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="a96d9-120">websiteUrl</span></span> |   <span data-ttu-id="a96d9-121">string</span><span class="sxs-lookup"><span data-stu-id="a96d9-121">string</span></span> |  <span data-ttu-id="a96d9-122">显示选项卡团队之外的内容的 Url。</span><span class="sxs-lookup"><span data-stu-id="a96d9-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="a96d9-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a96d9-123">JSON representation</span></span>

<span data-ttu-id="a96d9-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a96d9-124">The following is a JSON representation of the resource.</span></span>
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

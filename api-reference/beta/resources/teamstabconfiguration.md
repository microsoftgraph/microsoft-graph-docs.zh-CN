---
title: teamsTabConfiguration 资源类型 （打开类型）
description: 确定内容的选项卡的设置。
ms.openlocfilehash: b9a638692302dc8d301c3b14e50096b08891d821
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042709"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="32691-103">teamsTabConfiguration 资源类型 （打开类型）</span><span class="sxs-lookup"><span data-stu-id="32691-103">teamsTabConfiguration resource type (Open Type)</span></span>

> <span data-ttu-id="32691-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="32691-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32691-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="32691-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32691-106">确定内容的[选项卡上](teamstab.md)的设置。选项卡以交互方式配置时，此信息由选项卡提供程序应用程序设置。</span><span class="sxs-lookup"><span data-stu-id="32691-106">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="32691-107">除了下面的属性中，某些选项卡提供程序应用程序指定其他自定义属性。</span><span class="sxs-lookup"><span data-stu-id="32691-107">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="32691-108">属性</span><span class="sxs-lookup"><span data-stu-id="32691-108">Properties</span></span>

|<span data-ttu-id="32691-109">属性</span><span class="sxs-lookup"><span data-stu-id="32691-109">Property</span></span>|<span data-ttu-id="32691-110">类型</span><span class="sxs-lookup"><span data-stu-id="32691-110">Type</span></span>|<span data-ttu-id="32691-111">说明</span><span class="sxs-lookup"><span data-stu-id="32691-111">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="32691-112">entityId</span><span class="sxs-lookup"><span data-stu-id="32691-112">entityId</span></span>   |   <span data-ttu-id="32691-113">string</span><span class="sxs-lookup"><span data-stu-id="32691-113">string</span></span> |  <span data-ttu-id="32691-114">选项卡上的服务提供商托管实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="32691-114">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="32691-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="32691-115">contentUrl</span></span> |   <span data-ttu-id="32691-116">string</span><span class="sxs-lookup"><span data-stu-id="32691-116">string</span></span> |  <span data-ttu-id="32691-117">用于呈现团队中的选项卡内容的 Url。</span><span class="sxs-lookup"><span data-stu-id="32691-117">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="32691-118">必需。</span><span class="sxs-lookup"><span data-stu-id="32691-118">Required.</span></span>    |
|  <span data-ttu-id="32691-119">removeUrl</span><span class="sxs-lookup"><span data-stu-id="32691-119">removeUrl</span></span>  |   <span data-ttu-id="32691-120">string</span><span class="sxs-lookup"><span data-stu-id="32691-120">string</span></span> |  <span data-ttu-id="32691-121">使用团队客户端中移除一个选项卡时调用团队客户端的 Url。</span><span class="sxs-lookup"><span data-stu-id="32691-121">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="32691-122">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="32691-122">websiteUrl</span></span> |   <span data-ttu-id="32691-123">string</span><span class="sxs-lookup"><span data-stu-id="32691-123">string</span></span> |  <span data-ttu-id="32691-124">显示选项卡团队之外的内容的 Url。</span><span class="sxs-lookup"><span data-stu-id="32691-124">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="32691-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32691-125">JSON representation</span></span>

<span data-ttu-id="32691-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32691-126">The following is a JSON representation of the resource.</span></span>
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

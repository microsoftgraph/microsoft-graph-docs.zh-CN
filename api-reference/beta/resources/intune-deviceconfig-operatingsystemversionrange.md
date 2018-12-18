---
title: operatingSystemVersionRange 资源类型
description: 操作系统版本范围。
author: tfitzmac
ms.openlocfilehash: b853e71b2d8f66d24122afb51cea97fc6a8f8d7e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331162"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="e53ff-103">operatingSystemVersionRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="e53ff-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="e53ff-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e53ff-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e53ff-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e53ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e53ff-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e53ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e53ff-107">操作系统版本范围。</span><span class="sxs-lookup"><span data-stu-id="e53ff-107">Operating System version range.</span></span>
## <a name="properties"></a><span data-ttu-id="e53ff-108">属性</span><span class="sxs-lookup"><span data-stu-id="e53ff-108">Properties</span></span>
|<span data-ttu-id="e53ff-109">属性</span><span class="sxs-lookup"><span data-stu-id="e53ff-109">Property</span></span>|<span data-ttu-id="e53ff-110">类型</span><span class="sxs-lookup"><span data-stu-id="e53ff-110">Type</span></span>|<span data-ttu-id="e53ff-111">说明</span><span class="sxs-lookup"><span data-stu-id="e53ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e53ff-112">说明</span><span class="sxs-lookup"><span data-stu-id="e53ff-112">description</span></span>|<span data-ttu-id="e53ff-113">字符串</span><span class="sxs-lookup"><span data-stu-id="e53ff-113">String</span></span>|<span data-ttu-id="e53ff-114">此范围 （如有效 1702年生成） 的说明</span><span class="sxs-lookup"><span data-stu-id="e53ff-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="e53ff-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="e53ff-115">lowestVersion</span></span>|<span data-ttu-id="e53ff-116">字符串</span><span class="sxs-lookup"><span data-stu-id="e53ff-116">String</span></span>|<span data-ttu-id="e53ff-117">最低非独占此范围包含版本。</span><span class="sxs-lookup"><span data-stu-id="e53ff-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="e53ff-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="e53ff-118">highestVersion</span></span>|<span data-ttu-id="e53ff-119">字符串</span><span class="sxs-lookup"><span data-stu-id="e53ff-119">String</span></span>|<span data-ttu-id="e53ff-120">包含此范围的最高非独占版本。</span><span class="sxs-lookup"><span data-stu-id="e53ff-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e53ff-121">Relationships</span><span class="sxs-lookup"><span data-stu-id="e53ff-121">Relationships</span></span>
<span data-ttu-id="e53ff-122">无</span><span class="sxs-lookup"><span data-stu-id="e53ff-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e53ff-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e53ff-123">JSON Representation</span></span>
<span data-ttu-id="e53ff-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e53ff-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```






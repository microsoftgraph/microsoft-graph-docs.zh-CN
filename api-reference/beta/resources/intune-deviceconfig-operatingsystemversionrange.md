---
title: operatingSystemVersionRange 资源类型
description: 操作系统版本范围。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aaac008b013a8bf2cfd1a88d1fab06a523abb949
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398525"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="5c10a-103">operatingSystemVersionRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c10a-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="5c10a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5c10a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5c10a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5c10a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c10a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c10a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c10a-107">操作系统版本范围。</span><span class="sxs-lookup"><span data-stu-id="5c10a-107">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="5c10a-108">属性</span><span class="sxs-lookup"><span data-stu-id="5c10a-108">Properties</span></span>
|<span data-ttu-id="5c10a-109">属性</span><span class="sxs-lookup"><span data-stu-id="5c10a-109">Property</span></span>|<span data-ttu-id="5c10a-110">类型</span><span class="sxs-lookup"><span data-stu-id="5c10a-110">Type</span></span>|<span data-ttu-id="5c10a-111">说明</span><span class="sxs-lookup"><span data-stu-id="5c10a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c10a-112">说明</span><span class="sxs-lookup"><span data-stu-id="5c10a-112">description</span></span>|<span data-ttu-id="5c10a-113">String</span><span class="sxs-lookup"><span data-stu-id="5c10a-113">String</span></span>|<span data-ttu-id="5c10a-114">此范围 （如有效 1702年生成） 的说明</span><span class="sxs-lookup"><span data-stu-id="5c10a-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="5c10a-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="5c10a-115">lowestVersion</span></span>|<span data-ttu-id="5c10a-116">String</span><span class="sxs-lookup"><span data-stu-id="5c10a-116">String</span></span>|<span data-ttu-id="5c10a-117">最低非独占此范围包含版本。</span><span class="sxs-lookup"><span data-stu-id="5c10a-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="5c10a-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="5c10a-118">highestVersion</span></span>|<span data-ttu-id="5c10a-119">String</span><span class="sxs-lookup"><span data-stu-id="5c10a-119">String</span></span>|<span data-ttu-id="5c10a-120">包含此范围的最高非独占版本。</span><span class="sxs-lookup"><span data-stu-id="5c10a-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c10a-121">关系</span><span class="sxs-lookup"><span data-stu-id="5c10a-121">Relationships</span></span>
<span data-ttu-id="5c10a-122">无</span><span class="sxs-lookup"><span data-stu-id="5c10a-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c10a-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c10a-123">JSON Representation</span></span>
<span data-ttu-id="5c10a-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c10a-124">Here is a JSON representation of the resource.</span></span>
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





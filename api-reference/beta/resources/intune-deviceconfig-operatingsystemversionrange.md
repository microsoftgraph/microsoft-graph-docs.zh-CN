---
title: operatingSystemVersionRange 资源类型
description: 操作系统版本范围。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20a52b813de13b51fcf94a93fa440337e7123f02
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525955"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="8e096-103">operatingSystemVersionRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e096-103">operatingSystemVersionRange resource type</span></span>

<span data-ttu-id="8e096-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8e096-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e096-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8e096-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e096-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e096-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e096-107">操作系统版本范围。</span><span class="sxs-lookup"><span data-stu-id="8e096-107">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="8e096-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e096-108">Properties</span></span>
|<span data-ttu-id="8e096-109">属性</span><span class="sxs-lookup"><span data-stu-id="8e096-109">Property</span></span>|<span data-ttu-id="8e096-110">类型</span><span class="sxs-lookup"><span data-stu-id="8e096-110">Type</span></span>|<span data-ttu-id="8e096-111">说明</span><span class="sxs-lookup"><span data-stu-id="8e096-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e096-112">说明</span><span class="sxs-lookup"><span data-stu-id="8e096-112">description</span></span>|<span data-ttu-id="8e096-113">String</span><span class="sxs-lookup"><span data-stu-id="8e096-113">String</span></span>|<span data-ttu-id="8e096-114">此范围的说明（例如，有效的1702版本）</span><span class="sxs-lookup"><span data-stu-id="8e096-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="8e096-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="8e096-115">lowestVersion</span></span>|<span data-ttu-id="8e096-116">String</span><span class="sxs-lookup"><span data-stu-id="8e096-116">String</span></span>|<span data-ttu-id="8e096-117">此范围包含的最低包含版本。</span><span class="sxs-lookup"><span data-stu-id="8e096-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="8e096-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="8e096-118">highestVersion</span></span>|<span data-ttu-id="8e096-119">String</span><span class="sxs-lookup"><span data-stu-id="8e096-119">String</span></span>|<span data-ttu-id="8e096-120">此范围包含的最高包含版本。</span><span class="sxs-lookup"><span data-stu-id="8e096-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e096-121">关系</span><span class="sxs-lookup"><span data-stu-id="8e096-121">Relationships</span></span>
<span data-ttu-id="8e096-122">无</span><span class="sxs-lookup"><span data-stu-id="8e096-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e096-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e096-123">JSON Representation</span></span>
<span data-ttu-id="8e096-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e096-124">Here is a JSON representation of the resource.</span></span>
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




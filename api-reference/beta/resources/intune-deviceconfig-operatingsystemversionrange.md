---
title: operatingSystemVersionRange 资源类型
description: 操作系统版本范围。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e9019150efed2f52f884746d7c62f1d7e5a35e83
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293953"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="3ea43-103">operatingSystemVersionRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ea43-103">operatingSystemVersionRange resource type</span></span>

<span data-ttu-id="3ea43-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ea43-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ea43-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3ea43-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ea43-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ea43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ea43-107">操作系统版本范围。</span><span class="sxs-lookup"><span data-stu-id="3ea43-107">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="3ea43-108">属性</span><span class="sxs-lookup"><span data-stu-id="3ea43-108">Properties</span></span>
|<span data-ttu-id="3ea43-109">属性</span><span class="sxs-lookup"><span data-stu-id="3ea43-109">Property</span></span>|<span data-ttu-id="3ea43-110">类型</span><span class="sxs-lookup"><span data-stu-id="3ea43-110">Type</span></span>|<span data-ttu-id="3ea43-111">说明</span><span class="sxs-lookup"><span data-stu-id="3ea43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ea43-112">说明</span><span class="sxs-lookup"><span data-stu-id="3ea43-112">description</span></span>|<span data-ttu-id="3ea43-113">字符串</span><span class="sxs-lookup"><span data-stu-id="3ea43-113">String</span></span>|<span data-ttu-id="3ea43-114">此范围的说明 (例如，有效的1702版本) </span><span class="sxs-lookup"><span data-stu-id="3ea43-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="3ea43-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="3ea43-115">lowestVersion</span></span>|<span data-ttu-id="3ea43-116">字符串</span><span class="sxs-lookup"><span data-stu-id="3ea43-116">String</span></span>|<span data-ttu-id="3ea43-117">此范围包含的最低包含版本。</span><span class="sxs-lookup"><span data-stu-id="3ea43-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="3ea43-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="3ea43-118">highestVersion</span></span>|<span data-ttu-id="3ea43-119">字符串</span><span class="sxs-lookup"><span data-stu-id="3ea43-119">String</span></span>|<span data-ttu-id="3ea43-120">此范围包含的最高包含版本。</span><span class="sxs-lookup"><span data-stu-id="3ea43-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ea43-121">关系</span><span class="sxs-lookup"><span data-stu-id="3ea43-121">Relationships</span></span>
<span data-ttu-id="3ea43-122">无</span><span class="sxs-lookup"><span data-stu-id="3ea43-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ea43-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ea43-123">JSON Representation</span></span>
<span data-ttu-id="3ea43-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ea43-124">Here is a JSON representation of the resource.</span></span>
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





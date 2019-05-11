---
title: windowsInformationProtectionResourceCollection 资源类型
description: Windows 信息保护资源集合
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f5a31f85b70095975d1692e2a0aff175df12512
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940566"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="edad4-103">windowsInformationProtectionResourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="edad4-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="edad4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="edad4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edad4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="edad4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edad4-106">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="edad4-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="edad4-107">属性</span><span class="sxs-lookup"><span data-stu-id="edad4-107">Properties</span></span>
|<span data-ttu-id="edad4-108">属性</span><span class="sxs-lookup"><span data-stu-id="edad4-108">Property</span></span>|<span data-ttu-id="edad4-109">类型</span><span class="sxs-lookup"><span data-stu-id="edad4-109">Type</span></span>|<span data-ttu-id="edad4-110">说明</span><span class="sxs-lookup"><span data-stu-id="edad4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edad4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="edad4-111">displayName</span></span>|<span data-ttu-id="edad4-112">String</span><span class="sxs-lookup"><span data-stu-id="edad4-112">String</span></span>|<span data-ttu-id="edad4-113">显示名称</span><span class="sxs-lookup"><span data-stu-id="edad4-113">Display name</span></span>|
|<span data-ttu-id="edad4-114">资源</span><span class="sxs-lookup"><span data-stu-id="edad4-114">resources</span></span>|<span data-ttu-id="edad4-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="edad4-115">String collection</span></span>|<span data-ttu-id="edad4-116">资源集合</span><span class="sxs-lookup"><span data-stu-id="edad4-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="edad4-117">关系</span><span class="sxs-lookup"><span data-stu-id="edad4-117">Relationships</span></span>
<span data-ttu-id="edad4-118">无</span><span class="sxs-lookup"><span data-stu-id="edad4-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="edad4-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edad4-119">JSON Representation</span></span>
<span data-ttu-id="edad4-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edad4-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```





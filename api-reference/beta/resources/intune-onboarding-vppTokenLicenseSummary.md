---
title: vppTokenLicenseSummary 资源类型
description: 令牌中给定应用的许可证摘要。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20d7c24c887ca97f3a5a9890f5089b745130055e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777873"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="8dc44-103">vppTokenLicenseSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="8dc44-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="8dc44-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8dc44-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dc44-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8dc44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dc44-106">令牌中给定应用的许可证摘要。</span><span class="sxs-lookup"><span data-stu-id="8dc44-106">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="8dc44-107">属性</span><span class="sxs-lookup"><span data-stu-id="8dc44-107">Properties</span></span>
|<span data-ttu-id="8dc44-108">属性</span><span class="sxs-lookup"><span data-stu-id="8dc44-108">Property</span></span>|<span data-ttu-id="8dc44-109">类型</span><span class="sxs-lookup"><span data-stu-id="8dc44-109">Type</span></span>|<span data-ttu-id="8dc44-110">说明</span><span class="sxs-lookup"><span data-stu-id="8dc44-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dc44-111">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="8dc44-111">vppTokenId</span></span>|<span data-ttu-id="8dc44-112">String</span><span class="sxs-lookup"><span data-stu-id="8dc44-112">String</span></span>|<span data-ttu-id="8dc44-113">VPP 令牌的标识符。</span><span class="sxs-lookup"><span data-stu-id="8dc44-113">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="8dc44-114">appleId</span><span class="sxs-lookup"><span data-stu-id="8dc44-114">appleId</span></span>|<span data-ttu-id="8dc44-115">String</span><span class="sxs-lookup"><span data-stu-id="8dc44-115">String</span></span>|<span data-ttu-id="8dc44-116">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="8dc44-116">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="8dc44-117">organizationName</span><span class="sxs-lookup"><span data-stu-id="8dc44-117">organizationName</span></span>|<span data-ttu-id="8dc44-118">String</span><span class="sxs-lookup"><span data-stu-id="8dc44-118">String</span></span>|<span data-ttu-id="8dc44-119">与 Apple Volume Purchase Program 令牌关联的组织。</span><span class="sxs-lookup"><span data-stu-id="8dc44-119">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="8dc44-120">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8dc44-120">availableLicenseCount</span></span>|<span data-ttu-id="8dc44-121">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc44-121">Int32</span></span>|<span data-ttu-id="8dc44-122">可用的 VPP 许可证数。</span><span class="sxs-lookup"><span data-stu-id="8dc44-122">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="8dc44-123">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8dc44-123">usedLicenseCount</span></span>|<span data-ttu-id="8dc44-124">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc44-124">Int32</span></span>|<span data-ttu-id="8dc44-125">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="8dc44-125">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8dc44-126">关系</span><span class="sxs-lookup"><span data-stu-id="8dc44-126">Relationships</span></span>
<span data-ttu-id="8dc44-127">无</span><span class="sxs-lookup"><span data-stu-id="8dc44-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8dc44-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8dc44-128">JSON Representation</span></span>
<span data-ttu-id="8dc44-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8dc44-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenLicenseSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenLicenseSummary",
  "vppTokenId": "String",
  "appleId": "String",
  "organizationName": "String",
  "availableLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```




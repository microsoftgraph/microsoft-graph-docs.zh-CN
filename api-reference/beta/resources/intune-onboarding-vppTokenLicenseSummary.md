---
title: vppTokenLicenseSummary 资源类型
description: 令牌中给定应用的许可证摘要。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f9c126323e0f5785752238ec64cfade2c34d5c24
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161059"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="5c970-103">vppTokenLicenseSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c970-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="5c970-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5c970-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c970-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c970-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c970-106">令牌中给定应用的许可证摘要。</span><span class="sxs-lookup"><span data-stu-id="5c970-106">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="5c970-107">属性</span><span class="sxs-lookup"><span data-stu-id="5c970-107">Properties</span></span>
|<span data-ttu-id="5c970-108">属性</span><span class="sxs-lookup"><span data-stu-id="5c970-108">Property</span></span>|<span data-ttu-id="5c970-109">类型</span><span class="sxs-lookup"><span data-stu-id="5c970-109">Type</span></span>|<span data-ttu-id="5c970-110">说明</span><span class="sxs-lookup"><span data-stu-id="5c970-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c970-111">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="5c970-111">vppTokenId</span></span>|<span data-ttu-id="5c970-112">String</span><span class="sxs-lookup"><span data-stu-id="5c970-112">String</span></span>|<span data-ttu-id="5c970-113">VPP 令牌的标识符。</span><span class="sxs-lookup"><span data-stu-id="5c970-113">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="5c970-114">appleId</span><span class="sxs-lookup"><span data-stu-id="5c970-114">appleId</span></span>|<span data-ttu-id="5c970-115">String</span><span class="sxs-lookup"><span data-stu-id="5c970-115">String</span></span>|<span data-ttu-id="5c970-116">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="5c970-116">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="5c970-117">organizationName</span><span class="sxs-lookup"><span data-stu-id="5c970-117">organizationName</span></span>|<span data-ttu-id="5c970-118">String</span><span class="sxs-lookup"><span data-stu-id="5c970-118">String</span></span>|<span data-ttu-id="5c970-119">与 Apple volume purchase Program 令牌关联的组织。</span><span class="sxs-lookup"><span data-stu-id="5c970-119">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="5c970-120">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="5c970-120">availableLicenseCount</span></span>|<span data-ttu-id="5c970-121">Int32</span><span class="sxs-lookup"><span data-stu-id="5c970-121">Int32</span></span>|<span data-ttu-id="5c970-122">可用的 VPP 许可证数。</span><span class="sxs-lookup"><span data-stu-id="5c970-122">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="5c970-123">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="5c970-123">usedLicenseCount</span></span>|<span data-ttu-id="5c970-124">Int32</span><span class="sxs-lookup"><span data-stu-id="5c970-124">Int32</span></span>|<span data-ttu-id="5c970-125">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="5c970-125">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c970-126">关系</span><span class="sxs-lookup"><span data-stu-id="5c970-126">Relationships</span></span>
<span data-ttu-id="5c970-127">无</span><span class="sxs-lookup"><span data-stu-id="5c970-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c970-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c970-128">JSON Representation</span></span>
<span data-ttu-id="5c970-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c970-129">Here is a JSON representation of the resource.</span></span>
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





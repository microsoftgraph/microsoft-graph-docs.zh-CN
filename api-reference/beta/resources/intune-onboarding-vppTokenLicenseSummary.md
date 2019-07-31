---
title: vppTokenLicenseSummary 资源类型
description: 令牌中给定应用的许可证摘要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20bb4e83d3b69a705c172464fd18df53d1678df7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997986"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="4ee0a-103">vppTokenLicenseSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ee0a-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="4ee0a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4ee0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ee0a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ee0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ee0a-106">令牌中给定应用的许可证摘要。</span><span class="sxs-lookup"><span data-stu-id="4ee0a-106">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="4ee0a-107">属性</span><span class="sxs-lookup"><span data-stu-id="4ee0a-107">Properties</span></span>
|<span data-ttu-id="4ee0a-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ee0a-108">Property</span></span>|<span data-ttu-id="4ee0a-109">类型</span><span class="sxs-lookup"><span data-stu-id="4ee0a-109">Type</span></span>|<span data-ttu-id="4ee0a-110">说明</span><span class="sxs-lookup"><span data-stu-id="4ee0a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ee0a-111">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="4ee0a-111">vppTokenId</span></span>|<span data-ttu-id="4ee0a-112">String</span><span class="sxs-lookup"><span data-stu-id="4ee0a-112">String</span></span>|<span data-ttu-id="4ee0a-113">VPP 令牌的标识符。</span><span class="sxs-lookup"><span data-stu-id="4ee0a-113">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="4ee0a-114">appleId</span><span class="sxs-lookup"><span data-stu-id="4ee0a-114">appleId</span></span>|<span data-ttu-id="4ee0a-115">String</span><span class="sxs-lookup"><span data-stu-id="4ee0a-115">String</span></span>|<span data-ttu-id="4ee0a-116">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="4ee0a-116">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="4ee0a-117">organizationName</span><span class="sxs-lookup"><span data-stu-id="4ee0a-117">organizationName</span></span>|<span data-ttu-id="4ee0a-118">String</span><span class="sxs-lookup"><span data-stu-id="4ee0a-118">String</span></span>|<span data-ttu-id="4ee0a-119">与 Apple Volume Purchase Program 令牌关联的组织。</span><span class="sxs-lookup"><span data-stu-id="4ee0a-119">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="4ee0a-120">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4ee0a-120">availableLicenseCount</span></span>|<span data-ttu-id="4ee0a-121">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee0a-121">Int32</span></span>|<span data-ttu-id="4ee0a-122">可用的 VPP 许可证数。</span><span class="sxs-lookup"><span data-stu-id="4ee0a-122">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="4ee0a-123">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4ee0a-123">usedLicenseCount</span></span>|<span data-ttu-id="4ee0a-124">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee0a-124">Int32</span></span>|<span data-ttu-id="4ee0a-125">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="4ee0a-125">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ee0a-126">关系</span><span class="sxs-lookup"><span data-stu-id="4ee0a-126">Relationships</span></span>
<span data-ttu-id="4ee0a-127">无</span><span class="sxs-lookup"><span data-stu-id="4ee0a-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ee0a-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ee0a-128">JSON Representation</span></span>
<span data-ttu-id="4ee0a-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ee0a-129">Here is a JSON representation of the resource.</span></span>
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






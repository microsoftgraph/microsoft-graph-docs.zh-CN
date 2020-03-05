---
title: vppTokenLicenseSummary 资源类型
description: 令牌中给定应用的许可证摘要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 47d56f27ac08d1b4ca657973cf6e5ae0690ba498
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527701"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="7019b-103">vppTokenLicenseSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="7019b-103">vppTokenLicenseSummary resource type</span></span>

<span data-ttu-id="7019b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7019b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7019b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7019b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7019b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7019b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7019b-107">令牌中给定应用的许可证摘要。</span><span class="sxs-lookup"><span data-stu-id="7019b-107">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="7019b-108">属性</span><span class="sxs-lookup"><span data-stu-id="7019b-108">Properties</span></span>
|<span data-ttu-id="7019b-109">属性</span><span class="sxs-lookup"><span data-stu-id="7019b-109">Property</span></span>|<span data-ttu-id="7019b-110">类型</span><span class="sxs-lookup"><span data-stu-id="7019b-110">Type</span></span>|<span data-ttu-id="7019b-111">说明</span><span class="sxs-lookup"><span data-stu-id="7019b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7019b-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="7019b-112">vppTokenId</span></span>|<span data-ttu-id="7019b-113">String</span><span class="sxs-lookup"><span data-stu-id="7019b-113">String</span></span>|<span data-ttu-id="7019b-114">VPP 令牌的标识符。</span><span class="sxs-lookup"><span data-stu-id="7019b-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="7019b-115">appleId</span><span class="sxs-lookup"><span data-stu-id="7019b-115">appleId</span></span>|<span data-ttu-id="7019b-116">String</span><span class="sxs-lookup"><span data-stu-id="7019b-116">String</span></span>|<span data-ttu-id="7019b-117">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="7019b-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="7019b-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="7019b-118">organizationName</span></span>|<span data-ttu-id="7019b-119">String</span><span class="sxs-lookup"><span data-stu-id="7019b-119">String</span></span>|<span data-ttu-id="7019b-120">与 Apple Volume Purchase Program 令牌关联的组织。</span><span class="sxs-lookup"><span data-stu-id="7019b-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="7019b-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7019b-121">availableLicenseCount</span></span>|<span data-ttu-id="7019b-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7019b-122">Int32</span></span>|<span data-ttu-id="7019b-123">可用的 VPP 许可证数。</span><span class="sxs-lookup"><span data-stu-id="7019b-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="7019b-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7019b-124">usedLicenseCount</span></span>|<span data-ttu-id="7019b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7019b-125">Int32</span></span>|<span data-ttu-id="7019b-126">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="7019b-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7019b-127">关系</span><span class="sxs-lookup"><span data-stu-id="7019b-127">Relationships</span></span>
<span data-ttu-id="7019b-128">无</span><span class="sxs-lookup"><span data-stu-id="7019b-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7019b-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7019b-129">JSON Representation</span></span>
<span data-ttu-id="7019b-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7019b-130">Here is a JSON representation of the resource.</span></span>
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




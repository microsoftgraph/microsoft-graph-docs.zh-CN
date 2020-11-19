---
title: vppTokenLicenseSummary 资源类型
description: 令牌中给定应用的许可证摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5182e9aebbefa1a1ce818e52cb442a8950b0b737
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301198"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="78db8-103">vppTokenLicenseSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="78db8-103">vppTokenLicenseSummary resource type</span></span>

<span data-ttu-id="78db8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78db8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78db8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="78db8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78db8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="78db8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78db8-107">令牌中给定应用的许可证摘要。</span><span class="sxs-lookup"><span data-stu-id="78db8-107">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="78db8-108">属性</span><span class="sxs-lookup"><span data-stu-id="78db8-108">Properties</span></span>
|<span data-ttu-id="78db8-109">属性</span><span class="sxs-lookup"><span data-stu-id="78db8-109">Property</span></span>|<span data-ttu-id="78db8-110">类型</span><span class="sxs-lookup"><span data-stu-id="78db8-110">Type</span></span>|<span data-ttu-id="78db8-111">Description</span><span class="sxs-lookup"><span data-stu-id="78db8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78db8-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="78db8-112">vppTokenId</span></span>|<span data-ttu-id="78db8-113">字符串</span><span class="sxs-lookup"><span data-stu-id="78db8-113">String</span></span>|<span data-ttu-id="78db8-114">VPP 令牌的标识符。</span><span class="sxs-lookup"><span data-stu-id="78db8-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="78db8-115">appleId</span><span class="sxs-lookup"><span data-stu-id="78db8-115">appleId</span></span>|<span data-ttu-id="78db8-116">String</span><span class="sxs-lookup"><span data-stu-id="78db8-116">String</span></span>|<span data-ttu-id="78db8-117">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="78db8-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="78db8-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="78db8-118">organizationName</span></span>|<span data-ttu-id="78db8-119">String</span><span class="sxs-lookup"><span data-stu-id="78db8-119">String</span></span>|<span data-ttu-id="78db8-120">与 Apple Volume Purchase Program 令牌关联的组织。</span><span class="sxs-lookup"><span data-stu-id="78db8-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="78db8-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="78db8-121">availableLicenseCount</span></span>|<span data-ttu-id="78db8-122">Int32</span><span class="sxs-lookup"><span data-stu-id="78db8-122">Int32</span></span>|<span data-ttu-id="78db8-123">可用的 VPP 许可证数。</span><span class="sxs-lookup"><span data-stu-id="78db8-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="78db8-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="78db8-124">usedLicenseCount</span></span>|<span data-ttu-id="78db8-125">Int32</span><span class="sxs-lookup"><span data-stu-id="78db8-125">Int32</span></span>|<span data-ttu-id="78db8-126">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="78db8-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78db8-127">关系</span><span class="sxs-lookup"><span data-stu-id="78db8-127">Relationships</span></span>
<span data-ttu-id="78db8-128">无</span><span class="sxs-lookup"><span data-stu-id="78db8-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78db8-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78db8-129">JSON Representation</span></span>
<span data-ttu-id="78db8-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78db8-130">Here is a JSON representation of the resource.</span></span>
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





---
title: vppTokenLicenseSummary 资源类型
description: 许可证令牌中的给定应用程序的摘要。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8fb84a549d95459db1e4b39c11b526f73db08752
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395179"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="57e61-103">vppTokenLicenseSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="57e61-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="57e61-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="57e61-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="57e61-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="57e61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57e61-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57e61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57e61-107">许可证令牌中的给定应用程序的摘要。</span><span class="sxs-lookup"><span data-stu-id="57e61-107">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="57e61-108">属性</span><span class="sxs-lookup"><span data-stu-id="57e61-108">Properties</span></span>
|<span data-ttu-id="57e61-109">属性</span><span class="sxs-lookup"><span data-stu-id="57e61-109">Property</span></span>|<span data-ttu-id="57e61-110">类型</span><span class="sxs-lookup"><span data-stu-id="57e61-110">Type</span></span>|<span data-ttu-id="57e61-111">说明</span><span class="sxs-lookup"><span data-stu-id="57e61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57e61-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="57e61-112">vppTokenId</span></span>|<span data-ttu-id="57e61-113">String</span><span class="sxs-lookup"><span data-stu-id="57e61-113">String</span></span>|<span data-ttu-id="57e61-114">VPP 令牌的标识符。</span><span class="sxs-lookup"><span data-stu-id="57e61-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="57e61-115">appleId</span><span class="sxs-lookup"><span data-stu-id="57e61-115">appleId</span></span>|<span data-ttu-id="57e61-116">String</span><span class="sxs-lookup"><span data-stu-id="57e61-116">String</span></span>|<span data-ttu-id="57e61-117">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="57e61-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="57e61-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="57e61-118">organizationName</span></span>|<span data-ttu-id="57e61-119">String</span><span class="sxs-lookup"><span data-stu-id="57e61-119">String</span></span>|<span data-ttu-id="57e61-120">与 Apple 卷购买程序令牌关联的组织。</span><span class="sxs-lookup"><span data-stu-id="57e61-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="57e61-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="57e61-121">availableLicenseCount</span></span>|<span data-ttu-id="57e61-122">Int32</span><span class="sxs-lookup"><span data-stu-id="57e61-122">Int32</span></span>|<span data-ttu-id="57e61-123">VPP 可用的许可证数量。</span><span class="sxs-lookup"><span data-stu-id="57e61-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="57e61-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="57e61-124">usedLicenseCount</span></span>|<span data-ttu-id="57e61-125">Int32</span><span class="sxs-lookup"><span data-stu-id="57e61-125">Int32</span></span>|<span data-ttu-id="57e61-126">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="57e61-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57e61-127">关系</span><span class="sxs-lookup"><span data-stu-id="57e61-127">Relationships</span></span>
<span data-ttu-id="57e61-128">无</span><span class="sxs-lookup"><span data-stu-id="57e61-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57e61-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57e61-129">JSON Representation</span></span>
<span data-ttu-id="57e61-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57e61-130">Here is a JSON representation of the resource.</span></span>
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





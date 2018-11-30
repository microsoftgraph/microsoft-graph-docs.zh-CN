---
title: vppTokenLicenseSummary 资源类型
description: 许可证令牌中的给定应用程序的摘要。
ms.openlocfilehash: fba888c706b21a796615bf9bc2ea79968d5ad6d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043130"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="7a99a-103">vppTokenLicenseSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a99a-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="7a99a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7a99a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a99a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7a99a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a99a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7a99a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a99a-107">许可证令牌中的给定应用程序的摘要。</span><span class="sxs-lookup"><span data-stu-id="7a99a-107">License summary of a given app in a token.</span></span>
## <a name="properties"></a><span data-ttu-id="7a99a-108">属性</span><span class="sxs-lookup"><span data-stu-id="7a99a-108">Properties</span></span>
|<span data-ttu-id="7a99a-109">属性</span><span class="sxs-lookup"><span data-stu-id="7a99a-109">Property</span></span>|<span data-ttu-id="7a99a-110">类型</span><span class="sxs-lookup"><span data-stu-id="7a99a-110">Type</span></span>|<span data-ttu-id="7a99a-111">说明</span><span class="sxs-lookup"><span data-stu-id="7a99a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a99a-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="7a99a-112">vppTokenId</span></span>|<span data-ttu-id="7a99a-113">字符串</span><span class="sxs-lookup"><span data-stu-id="7a99a-113">String</span></span>|<span data-ttu-id="7a99a-114">VPP 令牌的标识符。</span><span class="sxs-lookup"><span data-stu-id="7a99a-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="7a99a-115">appleId</span><span class="sxs-lookup"><span data-stu-id="7a99a-115">appleId</span></span>|<span data-ttu-id="7a99a-116">String</span><span class="sxs-lookup"><span data-stu-id="7a99a-116">String</span></span>|<span data-ttu-id="7a99a-117">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="7a99a-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="7a99a-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="7a99a-118">organizationName</span></span>|<span data-ttu-id="7a99a-119">String</span><span class="sxs-lookup"><span data-stu-id="7a99a-119">String</span></span>|<span data-ttu-id="7a99a-120">与 Apple 卷购买程序令牌关联的组织。</span><span class="sxs-lookup"><span data-stu-id="7a99a-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="7a99a-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7a99a-121">availableLicenseCount</span></span>|<span data-ttu-id="7a99a-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7a99a-122">Int32</span></span>|<span data-ttu-id="7a99a-123">VPP 可用的许可证数量。</span><span class="sxs-lookup"><span data-stu-id="7a99a-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="7a99a-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7a99a-124">usedLicenseCount</span></span>|<span data-ttu-id="7a99a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7a99a-125">Int32</span></span>|<span data-ttu-id="7a99a-126">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="7a99a-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a99a-127">Relationships</span><span class="sxs-lookup"><span data-stu-id="7a99a-127">Relationships</span></span>
<span data-ttu-id="7a99a-128">无</span><span class="sxs-lookup"><span data-stu-id="7a99a-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7a99a-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a99a-129">JSON Representation</span></span>
<span data-ttu-id="7a99a-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a99a-130">Here is a JSON representation of the resource.</span></span>
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






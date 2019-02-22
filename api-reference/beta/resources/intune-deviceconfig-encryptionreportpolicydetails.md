---
title: encryptionReportPolicyDetails 资源类型
description: 加密报告的策略详细信息
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9232acd2a155169385956b9d20b3011c963090a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177915"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="cecc9-103">encryptionReportPolicyDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="cecc9-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="cecc9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cecc9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cecc9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cecc9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cecc9-106">加密报告的策略详细信息</span><span class="sxs-lookup"><span data-stu-id="cecc9-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="cecc9-107">属性</span><span class="sxs-lookup"><span data-stu-id="cecc9-107">Properties</span></span>
|<span data-ttu-id="cecc9-108">属性</span><span class="sxs-lookup"><span data-stu-id="cecc9-108">Property</span></span>|<span data-ttu-id="cecc9-109">类型</span><span class="sxs-lookup"><span data-stu-id="cecc9-109">Type</span></span>|<span data-ttu-id="cecc9-110">说明</span><span class="sxs-lookup"><span data-stu-id="cecc9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cecc9-111">policyId</span><span class="sxs-lookup"><span data-stu-id="cecc9-111">policyId</span></span>|<span data-ttu-id="cecc9-112">字符串</span><span class="sxs-lookup"><span data-stu-id="cecc9-112">String</span></span>|<span data-ttu-id="cecc9-113">加密报告的策略 Id</span><span class="sxs-lookup"><span data-stu-id="cecc9-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="cecc9-114">policyName</span><span class="sxs-lookup"><span data-stu-id="cecc9-114">policyName</span></span>|<span data-ttu-id="cecc9-115">字符串</span><span class="sxs-lookup"><span data-stu-id="cecc9-115">String</span></span>|<span data-ttu-id="cecc9-116">加密报告的策略名称</span><span class="sxs-lookup"><span data-stu-id="cecc9-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="cecc9-117">关系</span><span class="sxs-lookup"><span data-stu-id="cecc9-117">Relationships</span></span>
<span data-ttu-id="cecc9-118">无</span><span class="sxs-lookup"><span data-stu-id="cecc9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cecc9-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cecc9-119">JSON Representation</span></span>
<span data-ttu-id="cecc9-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cecc9-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptionReportPolicyDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptionReportPolicyDetails",
  "policyId": "String",
  "policyName": "String"
}
```





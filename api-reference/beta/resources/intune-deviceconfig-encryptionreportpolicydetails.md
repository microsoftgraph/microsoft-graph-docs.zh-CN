---
title: encryptionReportPolicyDetails 资源类型
description: 加密报告的策略详细信息
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7271329a7536a6359bbc9662427e65e21ea39d8b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325608"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="3ff71-103">encryptionReportPolicyDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ff71-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="3ff71-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3ff71-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ff71-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ff71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ff71-106">加密报告的策略详细信息</span><span class="sxs-lookup"><span data-stu-id="3ff71-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="3ff71-107">属性</span><span class="sxs-lookup"><span data-stu-id="3ff71-107">Properties</span></span>
|<span data-ttu-id="3ff71-108">属性</span><span class="sxs-lookup"><span data-stu-id="3ff71-108">Property</span></span>|<span data-ttu-id="3ff71-109">类型</span><span class="sxs-lookup"><span data-stu-id="3ff71-109">Type</span></span>|<span data-ttu-id="3ff71-110">说明</span><span class="sxs-lookup"><span data-stu-id="3ff71-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ff71-111">policyId</span><span class="sxs-lookup"><span data-stu-id="3ff71-111">policyId</span></span>|<span data-ttu-id="3ff71-112">String</span><span class="sxs-lookup"><span data-stu-id="3ff71-112">String</span></span>|<span data-ttu-id="3ff71-113">加密报告的策略 Id</span><span class="sxs-lookup"><span data-stu-id="3ff71-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="3ff71-114">policyName</span><span class="sxs-lookup"><span data-stu-id="3ff71-114">policyName</span></span>|<span data-ttu-id="3ff71-115">String</span><span class="sxs-lookup"><span data-stu-id="3ff71-115">String</span></span>|<span data-ttu-id="3ff71-116">加密报告的策略名称</span><span class="sxs-lookup"><span data-stu-id="3ff71-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ff71-117">关系</span><span class="sxs-lookup"><span data-stu-id="3ff71-117">Relationships</span></span>
<span data-ttu-id="3ff71-118">无</span><span class="sxs-lookup"><span data-stu-id="3ff71-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ff71-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ff71-119">JSON Representation</span></span>
<span data-ttu-id="3ff71-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ff71-120">Here is a JSON representation of the resource.</span></span>
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




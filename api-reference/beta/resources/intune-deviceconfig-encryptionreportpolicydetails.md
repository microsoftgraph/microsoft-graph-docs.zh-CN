---
title: encryptionReportPolicyDetails 资源类型
description: 加密报告的策略详细信息
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c9903b54483fc6f77cd183abee0e54b10acf9cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556296"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="5a941-103">encryptionReportPolicyDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a941-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="5a941-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5a941-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a941-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5a941-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a941-106">加密报告的策略详细信息</span><span class="sxs-lookup"><span data-stu-id="5a941-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="5a941-107">属性</span><span class="sxs-lookup"><span data-stu-id="5a941-107">Properties</span></span>
|<span data-ttu-id="5a941-108">属性</span><span class="sxs-lookup"><span data-stu-id="5a941-108">Property</span></span>|<span data-ttu-id="5a941-109">类型</span><span class="sxs-lookup"><span data-stu-id="5a941-109">Type</span></span>|<span data-ttu-id="5a941-110">说明</span><span class="sxs-lookup"><span data-stu-id="5a941-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a941-111">policyId</span><span class="sxs-lookup"><span data-stu-id="5a941-111">policyId</span></span>|<span data-ttu-id="5a941-112">String</span><span class="sxs-lookup"><span data-stu-id="5a941-112">String</span></span>|<span data-ttu-id="5a941-113">加密报告的策略 Id</span><span class="sxs-lookup"><span data-stu-id="5a941-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="5a941-114">policyName</span><span class="sxs-lookup"><span data-stu-id="5a941-114">policyName</span></span>|<span data-ttu-id="5a941-115">String</span><span class="sxs-lookup"><span data-stu-id="5a941-115">String</span></span>|<span data-ttu-id="5a941-116">加密报告的策略名称</span><span class="sxs-lookup"><span data-stu-id="5a941-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a941-117">关系</span><span class="sxs-lookup"><span data-stu-id="5a941-117">Relationships</span></span>
<span data-ttu-id="5a941-118">无</span><span class="sxs-lookup"><span data-stu-id="5a941-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a941-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a941-119">JSON Representation</span></span>
<span data-ttu-id="5a941-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a941-120">Here is a JSON representation of the resource.</span></span>
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






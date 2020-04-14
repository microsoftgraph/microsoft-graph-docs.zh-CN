---
title: encryptionReportPolicyDetails 资源类型
description: 加密报告的策略详细信息
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8a92037429908af4ff53ea45b9b5f9b65a5a436
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460063"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="aaa31-103">encryptionReportPolicyDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="aaa31-103">encryptionReportPolicyDetails resource type</span></span>

<span data-ttu-id="aaa31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaa31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aaa31-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aaa31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aaa31-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aaa31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaa31-107">加密报告的策略详细信息</span><span class="sxs-lookup"><span data-stu-id="aaa31-107">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="aaa31-108">属性</span><span class="sxs-lookup"><span data-stu-id="aaa31-108">Properties</span></span>
|<span data-ttu-id="aaa31-109">属性</span><span class="sxs-lookup"><span data-stu-id="aaa31-109">Property</span></span>|<span data-ttu-id="aaa31-110">类型</span><span class="sxs-lookup"><span data-stu-id="aaa31-110">Type</span></span>|<span data-ttu-id="aaa31-111">说明</span><span class="sxs-lookup"><span data-stu-id="aaa31-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaa31-112">policyId</span><span class="sxs-lookup"><span data-stu-id="aaa31-112">policyId</span></span>|<span data-ttu-id="aaa31-113">String</span><span class="sxs-lookup"><span data-stu-id="aaa31-113">String</span></span>|<span data-ttu-id="aaa31-114">加密报告的策略 Id</span><span class="sxs-lookup"><span data-stu-id="aaa31-114">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="aaa31-115">policyName</span><span class="sxs-lookup"><span data-stu-id="aaa31-115">policyName</span></span>|<span data-ttu-id="aaa31-116">String</span><span class="sxs-lookup"><span data-stu-id="aaa31-116">String</span></span>|<span data-ttu-id="aaa31-117">加密报告的策略名称</span><span class="sxs-lookup"><span data-stu-id="aaa31-117">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="aaa31-118">关系</span><span class="sxs-lookup"><span data-stu-id="aaa31-118">Relationships</span></span>
<span data-ttu-id="aaa31-119">无</span><span class="sxs-lookup"><span data-stu-id="aaa31-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aaa31-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aaa31-120">JSON Representation</span></span>
<span data-ttu-id="aaa31-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aaa31-121">Here is a JSON representation of the resource.</span></span>
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




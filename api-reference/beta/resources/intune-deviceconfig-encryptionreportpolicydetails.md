---
title: encryptionReportPolicyDetails 资源类型
description: 加密报告的策略详细信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 874af3d0bf98cbfc5884a4f3387eb8d55323acaf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294576"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="b49f4-103">encryptionReportPolicyDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="b49f4-103">encryptionReportPolicyDetails resource type</span></span>

<span data-ttu-id="b49f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b49f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b49f4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b49f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b49f4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b49f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b49f4-107">加密报告的策略详细信息</span><span class="sxs-lookup"><span data-stu-id="b49f4-107">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="b49f4-108">属性</span><span class="sxs-lookup"><span data-stu-id="b49f4-108">Properties</span></span>
|<span data-ttu-id="b49f4-109">属性</span><span class="sxs-lookup"><span data-stu-id="b49f4-109">Property</span></span>|<span data-ttu-id="b49f4-110">类型</span><span class="sxs-lookup"><span data-stu-id="b49f4-110">Type</span></span>|<span data-ttu-id="b49f4-111">Description</span><span class="sxs-lookup"><span data-stu-id="b49f4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b49f4-112">policyId</span><span class="sxs-lookup"><span data-stu-id="b49f4-112">policyId</span></span>|<span data-ttu-id="b49f4-113">字符串</span><span class="sxs-lookup"><span data-stu-id="b49f4-113">String</span></span>|<span data-ttu-id="b49f4-114">加密报告的策略 Id</span><span class="sxs-lookup"><span data-stu-id="b49f4-114">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="b49f4-115">policyName</span><span class="sxs-lookup"><span data-stu-id="b49f4-115">policyName</span></span>|<span data-ttu-id="b49f4-116">字符串</span><span class="sxs-lookup"><span data-stu-id="b49f4-116">String</span></span>|<span data-ttu-id="b49f4-117">加密报告的策略名称</span><span class="sxs-lookup"><span data-stu-id="b49f4-117">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="b49f4-118">关系</span><span class="sxs-lookup"><span data-stu-id="b49f4-118">Relationships</span></span>
<span data-ttu-id="b49f4-119">无</span><span class="sxs-lookup"><span data-stu-id="b49f4-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b49f4-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b49f4-120">JSON Representation</span></span>
<span data-ttu-id="b49f4-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b49f4-121">Here is a JSON representation of the resource.</span></span>
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





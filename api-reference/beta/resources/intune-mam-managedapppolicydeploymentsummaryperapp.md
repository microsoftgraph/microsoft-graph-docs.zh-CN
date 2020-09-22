---
title: managedAppPolicyDeploymentSummaryPerApp 资源类型
description: 表示每个应用的策略部署摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4e55ad697ca091ac650f47a92f384ec847d2d08
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030232"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="9a822-103">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a822-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="9a822-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a822-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a822-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9a822-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a822-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a822-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a822-107">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="9a822-107">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="9a822-108">属性</span><span class="sxs-lookup"><span data-stu-id="9a822-108">Properties</span></span>
|<span data-ttu-id="9a822-109">属性</span><span class="sxs-lookup"><span data-stu-id="9a822-109">Property</span></span>|<span data-ttu-id="9a822-110">类型</span><span class="sxs-lookup"><span data-stu-id="9a822-110">Type</span></span>|<span data-ttu-id="9a822-111">说明</span><span class="sxs-lookup"><span data-stu-id="9a822-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a822-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9a822-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="9a822-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9a822-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="9a822-114">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="9a822-114">Deployment of an app.</span></span>|
|<span data-ttu-id="9a822-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="9a822-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="9a822-116">Int32</span><span class="sxs-lookup"><span data-stu-id="9a822-116">Int32</span></span>|<span data-ttu-id="9a822-117">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="9a822-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a822-118">关系</span><span class="sxs-lookup"><span data-stu-id="9a822-118">Relationships</span></span>
<span data-ttu-id="9a822-119">无</span><span class="sxs-lookup"><span data-stu-id="9a822-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a822-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a822-120">JSON Representation</span></span>
<span data-ttu-id="9a822-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a822-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "String"
  },
  "configurationAppliedUserCount": 1024
}
```







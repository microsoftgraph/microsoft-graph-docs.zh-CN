---
title: managedAppPolicyDeploymentSummaryPerApp 资源类型
description: 表示每个应用的策略部署摘要。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 149a578f60ba5953f77c83ca2fbc3810931dffff
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262508"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="4cdd9-103">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="4cdd9-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="4cdd9-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4cdd9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cdd9-105">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="4cdd9-105">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="4cdd9-106">属性</span><span class="sxs-lookup"><span data-stu-id="4cdd9-106">Properties</span></span>
|<span data-ttu-id="4cdd9-107">属性</span><span class="sxs-lookup"><span data-stu-id="4cdd9-107">Property</span></span>|<span data-ttu-id="4cdd9-108">类型</span><span class="sxs-lookup"><span data-stu-id="4cdd9-108">Type</span></span>|<span data-ttu-id="4cdd9-109">说明</span><span class="sxs-lookup"><span data-stu-id="4cdd9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cdd9-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="4cdd9-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="4cdd9-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="4cdd9-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="4cdd9-112">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="4cdd9-112">Deployment of an app.</span></span>|
|<span data-ttu-id="4cdd9-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="4cdd9-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="4cdd9-114">Int32</span><span class="sxs-lookup"><span data-stu-id="4cdd9-114">Int32</span></span>|<span data-ttu-id="4cdd9-115">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="4cdd9-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cdd9-116">关系</span><span class="sxs-lookup"><span data-stu-id="4cdd9-116">Relationships</span></span>
<span data-ttu-id="4cdd9-117">无</span><span class="sxs-lookup"><span data-stu-id="4cdd9-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cdd9-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cdd9-118">JSON Representation</span></span>
<span data-ttu-id="4cdd9-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cdd9-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "configurationAppliedUserCount": 1024
}
```




---
title: managedAppPolicyDeploymentSummaryPerApp 资源类型
description: 表示每个应用的策略部署摘要。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84befe8b98b2e0e6883328c09bdee16e2720300d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037938"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="5fbfa-103">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="5fbfa-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="5fbfa-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5fbfa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fbfa-105">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="5fbfa-105">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="5fbfa-106">属性</span><span class="sxs-lookup"><span data-stu-id="5fbfa-106">Properties</span></span>
|<span data-ttu-id="5fbfa-107">属性</span><span class="sxs-lookup"><span data-stu-id="5fbfa-107">Property</span></span>|<span data-ttu-id="5fbfa-108">类型</span><span class="sxs-lookup"><span data-stu-id="5fbfa-108">Type</span></span>|<span data-ttu-id="5fbfa-109">说明</span><span class="sxs-lookup"><span data-stu-id="5fbfa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fbfa-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5fbfa-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="5fbfa-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5fbfa-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="5fbfa-112">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="5fbfa-112">Deployment of an app.</span></span>|
|<span data-ttu-id="5fbfa-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="5fbfa-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="5fbfa-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbfa-114">Int32</span></span>|<span data-ttu-id="5fbfa-115">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="5fbfa-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fbfa-116">关系</span><span class="sxs-lookup"><span data-stu-id="5fbfa-116">Relationships</span></span>
<span data-ttu-id="5fbfa-117">无</span><span class="sxs-lookup"><span data-stu-id="5fbfa-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fbfa-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5fbfa-118">JSON Representation</span></span>
<span data-ttu-id="5fbfa-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fbfa-119">Here is a JSON representation of the resource.</span></span>
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




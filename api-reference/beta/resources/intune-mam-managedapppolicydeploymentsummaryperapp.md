---
title: managedAppPolicyDeploymentSummaryPerApp 资源类型
description: 表示每个应用的策略部署摘要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f051c36a7d14a75b6a85a9352a6188756d0545ad
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940713"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="1af5a-103">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="1af5a-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="1af5a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1af5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1af5a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1af5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1af5a-106">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="1af5a-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="1af5a-107">属性</span><span class="sxs-lookup"><span data-stu-id="1af5a-107">Properties</span></span>
|<span data-ttu-id="1af5a-108">属性</span><span class="sxs-lookup"><span data-stu-id="1af5a-108">Property</span></span>|<span data-ttu-id="1af5a-109">类型</span><span class="sxs-lookup"><span data-stu-id="1af5a-109">Type</span></span>|<span data-ttu-id="1af5a-110">说明</span><span class="sxs-lookup"><span data-stu-id="1af5a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1af5a-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="1af5a-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="1af5a-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="1af5a-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="1af5a-113">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="1af5a-113">Deployment of an app.</span></span>|
|<span data-ttu-id="1af5a-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="1af5a-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="1af5a-115">Int32</span><span class="sxs-lookup"><span data-stu-id="1af5a-115">Int32</span></span>|<span data-ttu-id="1af5a-116">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="1af5a-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1af5a-117">关系</span><span class="sxs-lookup"><span data-stu-id="1af5a-117">Relationships</span></span>
<span data-ttu-id="1af5a-118">无</span><span class="sxs-lookup"><span data-stu-id="1af5a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1af5a-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1af5a-119">JSON Representation</span></span>
<span data-ttu-id="1af5a-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1af5a-120">Here is a JSON representation of the resource.</span></span>
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





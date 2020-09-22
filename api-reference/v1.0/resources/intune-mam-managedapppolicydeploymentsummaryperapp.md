---
title: managedAppPolicyDeploymentSummaryPerApp 资源类型
description: 表示每个应用的策略部署摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b7082c3f3b1bd4d52970f2af223c55770c686be0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041292"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="1a762-103">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a762-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="1a762-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a762-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a762-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a762-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a762-106">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="1a762-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="1a762-107">属性</span><span class="sxs-lookup"><span data-stu-id="1a762-107">Properties</span></span>
|<span data-ttu-id="1a762-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a762-108">Property</span></span>|<span data-ttu-id="1a762-109">类型</span><span class="sxs-lookup"><span data-stu-id="1a762-109">Type</span></span>|<span data-ttu-id="1a762-110">说明</span><span class="sxs-lookup"><span data-stu-id="1a762-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a762-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="1a762-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="1a762-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="1a762-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="1a762-113">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="1a762-113">Deployment of an app.</span></span>|
|<span data-ttu-id="1a762-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="1a762-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="1a762-115">Int32</span><span class="sxs-lookup"><span data-stu-id="1a762-115">Int32</span></span>|<span data-ttu-id="1a762-116">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="1a762-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a762-117">关系</span><span class="sxs-lookup"><span data-stu-id="1a762-117">Relationships</span></span>
<span data-ttu-id="1a762-118">无</span><span class="sxs-lookup"><span data-stu-id="1a762-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a762-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a762-119">JSON Representation</span></span>
<span data-ttu-id="1a762-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a762-120">Here is a JSON representation of the resource.</span></span>
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










---
title: managedAppPolicyDeploymentSummaryPerApp 资源类型
description: 表示每个应用的策略部署摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a1bcf69e4a8d24af3f0ada2ceae5730cc0cfdc18
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752327"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="6633c-103">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="6633c-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="6633c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6633c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6633c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6633c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6633c-106">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="6633c-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="6633c-107">属性</span><span class="sxs-lookup"><span data-stu-id="6633c-107">Properties</span></span>
|<span data-ttu-id="6633c-108">属性</span><span class="sxs-lookup"><span data-stu-id="6633c-108">Property</span></span>|<span data-ttu-id="6633c-109">类型</span><span class="sxs-lookup"><span data-stu-id="6633c-109">Type</span></span>|<span data-ttu-id="6633c-110">Description</span><span class="sxs-lookup"><span data-stu-id="6633c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6633c-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="6633c-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="6633c-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="6633c-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="6633c-113">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="6633c-113">Deployment of an app.</span></span>|
|<span data-ttu-id="6633c-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="6633c-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="6633c-115">Int32</span><span class="sxs-lookup"><span data-stu-id="6633c-115">Int32</span></span>|<span data-ttu-id="6633c-116">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="6633c-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6633c-117">关系</span><span class="sxs-lookup"><span data-stu-id="6633c-117">Relationships</span></span>
<span data-ttu-id="6633c-118">无</span><span class="sxs-lookup"><span data-stu-id="6633c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6633c-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6633c-119">JSON Representation</span></span>
<span data-ttu-id="6633c-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6633c-120">Here is a JSON representation of the resource.</span></span>
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





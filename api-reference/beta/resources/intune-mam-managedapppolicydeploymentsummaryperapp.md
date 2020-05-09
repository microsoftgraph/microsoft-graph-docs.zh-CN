---
title: managedAppPolicyDeploymentSummaryPerApp 资源类型
description: 表示每个应用的策略部署摘要。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e4f9c3af886afa5c5d0e78f23bb55d9f764b0298
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177406"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="5aa98-103">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="5aa98-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="5aa98-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aa98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5aa98-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5aa98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5aa98-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5aa98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5aa98-107">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="5aa98-107">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="5aa98-108">属性</span><span class="sxs-lookup"><span data-stu-id="5aa98-108">Properties</span></span>
|<span data-ttu-id="5aa98-109">属性</span><span class="sxs-lookup"><span data-stu-id="5aa98-109">Property</span></span>|<span data-ttu-id="5aa98-110">类型</span><span class="sxs-lookup"><span data-stu-id="5aa98-110">Type</span></span>|<span data-ttu-id="5aa98-111">说明</span><span class="sxs-lookup"><span data-stu-id="5aa98-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5aa98-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5aa98-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="5aa98-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5aa98-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="5aa98-114">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="5aa98-114">Deployment of an app.</span></span>|
|<span data-ttu-id="5aa98-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="5aa98-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="5aa98-116">Int32</span><span class="sxs-lookup"><span data-stu-id="5aa98-116">Int32</span></span>|<span data-ttu-id="5aa98-117">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="5aa98-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5aa98-118">关系</span><span class="sxs-lookup"><span data-stu-id="5aa98-118">Relationships</span></span>
<span data-ttu-id="5aa98-119">无</span><span class="sxs-lookup"><span data-stu-id="5aa98-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5aa98-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5aa98-120">JSON Representation</span></span>
<span data-ttu-id="5aa98-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5aa98-121">Here is a JSON representation of the resource.</span></span>
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



